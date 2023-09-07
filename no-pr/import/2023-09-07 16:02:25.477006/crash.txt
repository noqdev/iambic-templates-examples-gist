Traceback (most recent call last):
  File "/app/iambic/plugins/v0_1_0/github/github.py", line 734, in wrapped_workflow_func
    template_changes = workflow_func(
  File "/app/iambic/plugins/v0_1_0/github/github.py", line 1009, in _handle_import
    raise e
  File "/app/iambic/plugins/v0_1_0/github/github.py", line 999, in _handle_import
    asyncio.run(config.run_import(exe_message, repo_dir))
  File "/Python-3.10.12/Lib/asyncio/runners.py", line 44, in run
    return loop.run_until_complete(main)
  File "/Python-3.10.12/Lib/asyncio/base_events.py", line 649, in run_until_complete
    return future.result()
  File "/app/iambic/config/dynamic_config.py", line 273, in run_import
    await asyncio.gather(*tasks)
  File "/app/iambic/plugins/v0_1_0/azure_ad/handlers.py", line 65, in import_azure_ad_resources
    await asyncio.gather(*collector_tasks)
  File "/app/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py", line 61, in collect_org_groups
    groups = await list_groups(azure_organization)
  File "/app/iambic/plugins/v0_1_0/azure_ad/group/utils.py", line 96, in list_groups
    groups = await retry_controller(fn)
  File "/app/iambic/core/utils.py", line 663, in __call__
    raise e
  File "/app/iambic/core/utils.py", line 657, in __call__
    res = await func(*args, **kwargs)
  File "/app/iambic/plugins/v0_1_0/azure_ad/models.py", line 119, in list
    return await self._make_request("list", endpoint, **kwargs)
  File "/app/iambic/plugins/v0_1_0/azure_ad/models.py", line 62, in _make_request
    await self.set_azure_access_token()
  File "/app/iambic/plugins/v0_1_0/azure_ad/models.py", line 56, in set_azure_access_token
    raise Exception("Access token was not successfully acquired")
Exception: Access token was not successfully acquired
