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
  File "/app/iambic/config/dynamic_config.py", line 228, in run_import
    await asyncio.gather(*tasks)
  File "/app/iambic/plugins/v0_1_0/azure_ad/handlers.py", line 72, in import_azure_ad_resources
    await asyncio.gather(*generator_tasks)
  File "/app/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py", line 83, in generate_user_templates
    existing_template_map = await get_existing_template_map(
                            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/template_generation.py", line 32, in get_existing_template_map
    templates = load_templates(await gather_templates(repo_dir, template_type))
                               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/utils.py", line 161, in gather_templates
    file_paths = await gather_limit(
                 ^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/aio_utils/__init__.py", line 70, in gather_limit
    ret[pos[x]] = x.result()
                  ^^^^^^^^^^
  File "/app/iambic/core/utils.py", line 132, in file_regex_search
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
FileNotFoundError: [Errno 2] No such file or directory: '/tmp/lambda8wln37q7/.iambic/repos/resources/google_workspace/group/iambic.org/iambic_test_group.yaml'
