Traceback (most recent call last):
  File "/app/iambic/plugins/v0_1_0/github/github.py", line 734, in wrapped_workflow_func
    template_changes = workflow_func(
  File "/app/iambic/plugins/v0_1_0/github/github.py", line 1009, in _handle_import
    raise e
  File "/app/iambic/plugins/v0_1_0/github/github.py", line 998, in _handle_import
    config = __get_config()
  File "/app/iambic/plugins/v0_1_0/github/github.py", line 867, in __get_config
    config = asyncio.run(load_config(config_path))
  File "/Python-3.10.12/Lib/asyncio/runners.py", line 44, in run
    return loop.run_until_complete(main)
  File "/Python-3.10.12/Lib/asyncio/base_events.py", line 649, in run_until_complete
    return future.result()
  File "/app/iambic/config/dynamic_config.py", line 497, in load_config
    return await process_config(
  File "/app/iambic/config/dynamic_config.py", line 559, in process_config
    await config.configure_plugins()
  File "/app/iambic/config/dynamic_config.py", line 378, in configure_plugins
    await plugin.async_load_callable(self.get_config_plugin(plugin))
  File "/app/iambic/plugins/v0_1_0/aws/handlers.py", line 93, in load
    orgs_accounts = await asyncio.gather(
  File "/app/iambic/plugins/v0_1_0/aws/models.py", line 786, in get_accounts
    session = await self.get_boto3_session()
  File "/app/iambic/plugins/v0_1_0/aws/models.py", line 222, in get_boto3_session
    boto3_session = await create_assume_role_session(
  File "/app/iambic/plugins/v0_1_0/aws/utils.py", line 353, in create_assume_role_session
    role = await aio_wrapper(sts.assume_role, **role_params)
  File "/app/iambic/core/utils.py", line 184, in aio_wrapper
    return await sync_to_async(fnc, thread_sensitive=thread_sensitive)(*args, **kwargs)
  File "/usr/local/lib/python3.10/site-packages/asgiref/sync.py", line 479, in __call__
    ret: _R = await loop.run_in_executor(
  File "/Python-3.10.12/Lib/concurrent/futures/thread.py", line 58, in run
    result = self.fn(*self.args, **self.kwargs)
  File "/usr/local/lib/python3.10/site-packages/asgiref/sync.py", line 538, in thread_handler
    return func(*args, **kwargs)
  File "/usr/local/lib/python3.10/site-packages/botocore/client.py", line 534, in _api_call
    return self._make_api_call(operation_name, kwargs)
  File "/usr/local/lib/python3.10/site-packages/botocore/client.py", line 976, in _make_api_call
    raise error_class(parsed_response, operation_name)
botocore.exceptions.ClientError: An error occurred (AccessDenied) when calling the AssumeRole operation: User: arn:aws:sts::580605962305:assumed-role/iambic_github_app_lambda_execution/iambic_github_app_webhook is not authorized to perform: sts:AssumeRole on resource: arn:aws:iam::580605962305:role/IambicHubRole
