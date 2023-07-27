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
  File "/app/iambic/plugins/v0_1_0/aws/handlers.py", line 419, in import_aws_resources
    tasks += await import_organization_resources(
             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/plugins/v0_1_0/aws/handlers.py", line 472, in import_organization_resources
    scp_template_map = await get_existing_template_map(
                       ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/template_generation.py", line 39, in get_existing_template_map
    await gather_templates(repo_dir, template_type), template_map
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/utils.py", line 167, in gather_templates
    file_paths = await gather_limit(
                 ^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/aio_utils/__init__.py", line 70, in gather_limit
    ret[pos[x]] = x.result()
                  ^^^^^^^^^^
  File "/app/iambic/core/utils.py", line 138, in file_regex_search
    async with aiofiles.open(file_path, mode="r") as f:
  File "/usr/local/lib/python3.11/site-packages/aiofiles/base.py", line 98, in __aenter__
    self._obj = await self._coro
                ^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/aiofiles/threadpool/__init__.py", line 97, in _open
    f = yield from loop.run_in_executor(executor, cb)
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Python-3.11.1/Lib/concurrent/futures/thread.py", line 58, in run
    result = self.fn(*self.args, **self.kwargs)
             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
FileNotFoundError: [Errno 2] No such file or directory: '/tmp/lambdaj119xqw3/.iambic/repos/resources/google_workspace/group/iambic.org/iambic_test_group_9bca5dc0_2351_4990_8c00_93302adfbd5f.yaml'
