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
  File "/app/iambic/plugins/v0_1_0/google_workspace/handlers.py", line 57, in import_google_resources
    await asyncio.gather(*collector_tasks)
  File "/app/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py", line 116, in collect_project_groups
    await asyncio.gather(
  File "/app/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py", line 73, in generate_domain_group_resource_files
    groups = await list_groups(domain, project)
             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/plugins/v0_1_0/google_workspace/group/utils.py", line 43, in list_groups
    group_template = await get_group_template(service, group, domain)
                     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/plugins/v0_1_0/google_workspace/group/models.py", line 285, in get_group_template
    members = await get_group_members(service, group)
              ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/iambic/plugins/v0_1_0/google_workspace/group/utils.py", line 331, in get_group_members
    return [
           ^
  File "/app/iambic/plugins/v0_1_0/google_workspace/group/utils.py", line 333, in <listcomp>
    email=member["email"],
          ~~~~~~^^^^^^^^^
KeyError: 'email'
