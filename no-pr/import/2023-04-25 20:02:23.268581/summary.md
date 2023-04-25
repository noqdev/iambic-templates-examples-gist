Traceback (most recent call last):
  File "/app/iambic/core/parser.py", line 115, in load_templates
    templates.append(template_cls(**template_dict))
                     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/models.py", line 84, in __init__
    super().__init__(*args, **kwargs)
  File "pydantic/main.py", line 341, in pydantic.main.BaseModel.__init__
pydantic.error_wrappers.ValidationError: 2 validation errors for AwsIamRoleTemplate
Properties -> PermissionsBoundary -> permissions_boundary_arn
  string does not match regex "(^arn:([^:]*):([^:]*):([^:]*):(|\*|[\d]{12}|cloudfront|aws|{{var.account_id}}):(.+)$)|^\*$" (type=value_error.str.regex; pattern=(^arn:([^:]*):([^:]*):([^:]*):(|\*|[\d]{12}|cloudfront|aws|{{var.account_id}}):(.+)$)|^\*$)
Properties -> PermissionsBoundary
  value is not a valid list (type=type_error.list)

The above exception was the direct cause of the following exception:

Traceback (most recent call last):
  File "/app/iambic/plugins/v0_1_0/github/github.py", line 558, in wrapped_workflow_func
    template_changes = workflow_func(repo_url, default_branch)
                       ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/plugins/v0_1_0/github/github.py", line 723, in _handle_import
    raise e
  File "/app/iambic/plugins/v0_1_0/github/github.py", line 713, in _handle_import
    asyncio.run(config.run_import(exe_message, repo_dir))
  File "/Python-3.11.1/Lib/asyncio/runners.py", line 190, in run
    return runner.run(main)
           ^^^^^^^^^^^^^^^^
  File "/Python-3.11.1/Lib/asyncio/runners.py", line 118, in run
    return self._loop.run_until_complete(task)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Python-3.11.1/Lib/asyncio/base_events.py", line 653, in run_until_complete
    return future.result()
           ^^^^^^^^^^^^^^^
  File "/app/iambic/config/dynamic_config.py", line 232, in run_import
    await asyncio.gather(*tasks)
  File "/app/iambic/plugins/v0_1_0/aws/handlers.py", line 399, in import_aws_resources
    iam_template_map = await get_existing_template_map(
                       ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/template_generation.py", line 34, in get_existing_template_map
    templates = load_templates(await gather_templates(repo_dir, template_type))
                ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/parser.py", line 132, in load_templates
    raise ValueError(
ValueError: /tmp/lambda957l6xlz/.iambic/repos/resources/aws/iam/role/iambic_test_spoke_account_1/awsreservedsso_iambic_test_8474_3179785f7326d1fc.yaml template has validation error. 
line 5: `properties.permissionsboundary` has type issue
