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
  File "/app/iambic/plugins/v0_1_0/aws/handlers.py", line 456, in import_aws_resources
    await asyncio.gather(*tasks)
  File "/app/iambic/plugins/v0_1_0/aws/handlers.py", line 332, in import_service_resources
    await asyncio.gather(*tasks)
  File "/app/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py", line 548, in collect_aws_roles
    await set_role_resource_inline_policies_semaphore.process(messages)
  File "/app/iambic/core/utils.py", line 218, in process
    return await asyncio.gather(
           ^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/utils.py", line 213, in handle_message
    return await self.callback_function(**kwargs)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py", line 205, in set_role_resource_inline_policies
    role_inline_policies = await get_role_inline_policies(role_name, iam_client)
                           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/plugins/v0_1_0/aws/iam/role/utils.py", line 71, in get_role_inline_policies
    policy_names = await get_role_inline_policy_names(role_name, iam_client)
                   ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/plugins/v0_1_0/aws/iam/role/utils.py", line 19, in get_role_inline_policy_names
    return await paginated_search(
           ^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/plugins/v0_1_0/aws/utils.py", line 105, in paginated_search
    response = await boto_crud_call(search_fnc, **search_kwargs)
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/plugins/v0_1_0/aws/utils.py", line 52, in boto_crud_call
    return await aio_wrapper(boto_fnc, **kwargs)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/utils.py", line 175, in aio_wrapper
    return await sync_to_async(fnc, thread_sensitive=thread_sensitive)(*args, **kwargs)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/asgiref/sync.py", line 479, in __call__
    ret: _R = await loop.run_in_executor(
              ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Python-3.11.1/Lib/concurrent/futures/thread.py", line 58, in run
    result = self.fn(*self.args, **self.kwargs)
             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/asgiref/sync.py", line 538, in thread_handler
    return func(*args, **kwargs)
           ^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/botocore/client.py", line 530, in _api_call
    return self._make_api_call(operation_name, kwargs)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/botocore/client.py", line 964, in _make_api_call
    raise error_class(parsed_response, operation_name)
botocore.errorfactory.NoSuchEntityException: An error occurred (NoSuchEntity) when calling the ListRolePolicies operation: The role with name AWSReservedSSO_iambic_test_2593_bfacde26c724719c cannot be found.
