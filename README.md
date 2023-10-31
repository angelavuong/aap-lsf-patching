# aap-lsf-patching

This demo will query for the LSF cluster for nodes with njobs == 0 and patch those servers. 

![image](https://github.com/angelavuong/aap-lsf-patching/blob/main/images/aap-lsf-patching.png)

**Workflow Job Templates:**
1. Query LSF job count and stop LSF jobs
- https://github.com/angelavuong/aap-lsf-patching/blob/main/lsf_stop_jobs.yml
- Enable Fact Storage

2. Patch RHEL servers
- https://github.com/angelavuong/aap-lsf-patching/blob/main/patch_rhel_hosts.yml
- Enable Fact Storage

3. Re-open LSF nodes
- https://github.com/angelavuong/aap-lsf-patching/blob/main/lsf_start_jobs.yml
- Enable Fact Storage

**Future additions:**
- Differentiate between master/worker LSF nodes
- Reboot servers that have been patched 
