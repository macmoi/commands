# Azure Pipelines Util Info


## Common Pipeline Variables.

These variables are used to construct pipelines using YAML files.
Normally during pipeline coding is necessary to have reference to
specific folders or locations inside the agent. Or access particular
predefined configs of the project. Those variables will be described here.


--------------

- `Build.ArtifactStagingDirectory`: makes a reference to `c:/agent_dir/1/a`
- `Build.BuildId`: The ID of the record for the completed build.
- `Build.BinariesDirectory`: Used as output for compiled binaries. `c:/agent_dir/1/b`
- `Build.ContainerId`: The ID of the container for the artifact. When an artifact is uploaded in the pipeline, it is added to a container that is specific for that particular artifact
- `Build.StagingDirectory`: Makes a reference to: `c:\agent_work\1\a`. Is where any artifact is copied before being pushed to their destination.
- `Pipeline.Workspace`: Workspace directory for a particular pipeline. Same value as `Agent.BuildDirectory`
- `Agent.BuildDirectory`: The local path on the agent where all folders for a given build pipeline are created. This variable has the same value as `Pipeline.Worspace`. Which is `/home/vsts/work/1` or `c:/agent_dir/1`

