# TestUnityCI
  
## Quick setup guide

### Basics
- Create a github repo and clone locally, as normal
- `git lfs install` to setup Git LFS
- Add [.gitignore](https://github.com/github/gitignore/blob/main/Unity.gitignore)
- Add [.gitattributes](https://gist.github.com/Srfigie/77b5c15bc5eb61733a74d34d10b3ed87)
- Add [main.yml](https://github.com/Prybh/TestUnityCI/blob/main/.github/workflows/main.yml)
- Submit

### CI Variables
- Go in Actions, in the last build and download the Unity_v20xx.x.ulf
- Go in Settings/Secrets/Actions
- Copy all the file content to a new secret UNITY_LICENSE
- Add a new secrets UNITY_EMAIL and UNITY_PASSWORD for your Unity account

### Deploy
- Disable compression for WebGL builds
- Submit first commit
- Go in Settings/Pages and select the gh-pages branch for the deploy
- Submit
  
## Links
 
.gitignore for Unity : https://github.com/github/gitignore/blob/main/Unity.gitignore  
Git LFS with Unity : https://adamwreed93.medium.com/how-to-set-up-git-lfs-into-your-unity-project-9fd276305fe7  
.gitattributes for Unity : https://gist.github.com/Srfigie/77b5c15bc5eb61733a74d34d10b3ed87  
  
GameCI docs : https://game.ci/docs/github/getting-started  
unity-actions : https://github.com/game-ci/unity-actions  
unity-license-activate : https://github.com/game-ci/unity-license-activate  
Example follow guide : https://github.com/yanniboi/RogueCI/wiki  
Example complete : https://github.com/yanniboi/RogueCI 
