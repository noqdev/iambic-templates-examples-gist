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
  File "/app/iambic/plugins/v0_1_0/aws/handlers.py", line 362, in import_aws_resources
    await asyncio.gather(*tasks)
  File "/app/iambic/plugins/v0_1_0/aws/handlers.py", line 273, in import_service_resources
    await asyncio.gather(*tasks)
  File "/app/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py", line 433, in collect_aws_roles
    existing_template_map = await get_existing_template_map(
                            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/template_generation.py", line 32, in get_existing_template_map
    templates = load_templates(await gather_templates(repo_dir, template_type))
                ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/core/parser.py", line 90, in load_templates
    with Pool(max(1, cpu_count() // 2)) as p:
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Python-3.11.1/Lib/multiprocessing/context.py", line 119, in Pool
    return Pool(processes, initializer, initargs, maxtasksperchild,
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Python-3.11.1/Lib/multiprocessing/pool.py", line 191, in __init__
    self._setup_queues()
  File "/Python-3.11.1/Lib/multiprocessing/pool.py", line 346, in _setup_queues
    self._inqueue = self._ctx.SimpleQueue()
                    ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Python-3.11.1/Lib/multiprocessing/context.py", line 113, in SimpleQueue
    return SimpleQueue(ctx=self.get_context())
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Python-3.11.1/Lib/multiprocessing/queues.py", line 341, in __init__
    self._rlock = ctx.Lock()
                  ^^^^^^^^^^
  File "/Python-3.11.1/Lib/multiprocessing/context.py", line 68, in Lock
    return Lock(ctx=self.get_context())
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Python-3.11.1/Lib/multiprocessing/synchronize.py", line 162, in __init__
    SemLock.__init__(self, SEMAPHORE, 1, 1, ctx=ctx)
  File "/Python-3.11.1/Lib/multiprocessing/synchronize.py", line 57, in __init__
    sl = self._semlock = _multiprocessing.SemLock(
                         ^^^^^^^^^^^^^^^^^^^^^^^^^
FileNotFoundError: [Errno 2] No such file or directory
