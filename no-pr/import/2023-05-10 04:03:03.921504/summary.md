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
  File "/app/iambic/plugins/v0_1_0/aws/handlers.py", line 429, in import_aws_resources
    await asyncio.gather(*tasks)
  File "/app/iambic/plugins/v0_1_0/aws/handlers.py", line 353, in import_identity_center_resources
    await import_service_resources(
  File "/app/iambic/plugins/v0_1_0/aws/handlers.py", line 312, in import_service_resources
    await asyncio.gather(
  File "/app/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py", line 550, in generate_aws_permission_set_templates
    resource_template = await create_templated_permission_set(
                        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py", line 372, in create_templated_permission_set
    PermissionSetProperties(**template_properties),
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/models.py", line 84, in __init__
    super().__init__(*args, **kwargs)
  File "pydantic/main.py", line 341, in pydantic.main.BaseModel.__init__
pydantic.error_wrappers.ValidationError: 1 validation error for PermissionSetProperties
PermissionsBoundary -> managed_policy_arn
  extra fields not permitted (type=value_error.extra)
