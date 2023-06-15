Traceback (most recent call last):
  File "/app/iambic/plugins/v0_1_0/github/github.py", line 647, in wrapped_workflow_func
    template_changes = workflow_func(repo_url, default_branch)
                       ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/plugins/v0_1_0/github/github.py", line 812, in _handle_import
    raise e
  File "/app/iambic/plugins/v0_1_0/github/github.py", line 802, in _handle_import
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
  File "/app/iambic/config/dynamic_config.py", line 245, in run_import
    await asyncio.gather(*tasks)
  File "/app/iambic/plugins/v0_1_0/aws/handlers.py", line 458, in import_aws_resources
    await asyncio.gather(*tasks)
  File "/app/iambic/plugins/v0_1_0/aws/handlers.py", line 335, in import_service_resources
    await asyncio.gather(
  File "/app/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py", line 605, in generate_aws_role_templates
    resource_template = await create_templated_role(
                        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py", line 435, in create_templated_role
    RoleProperties(**role_template_properties),
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/models.py", line 85, in __init__
    super().__init__(*args, **kwargs)
  File "pydantic/main.py", line 341, in pydantic.main.BaseModel.__init__
pydantic.error_wrappers.ValidationError: 1 validation error for RoleProperties
InlinePolicies -> 0 -> id
  extra fields not permitted (type=value_error.extra)
