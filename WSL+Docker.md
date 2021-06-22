# Setting _WSL+Docker_

Setting up of the WSL+Docker workspace. Some of the useful resources have been listed below:

- [WSL+Docker: Kubernetes on the Windows Desktop](https://kubernetes.io/blog/2020/05/21/wsl-docker-kubernetes-on-the-windows-desktop/)
- [Manual Installation Stepsfor WSL](https://docs.microsoft.com/en-us/windows/wsl/install-win10#manual-installation-steps)
- [Docker Desktop for Windows](https://hub.docker.com/editions/community/docker-ce-desktop-windows)

## Related threads to problems faced

- After the step of enabling SystemD, if running, **sudo minikube start --driver=none** gives an error. Try [this](https://discuss.kubernetes.io/t/problem-in-setting-up-kubernetes-in-wsl-failed-to-start-docker-service-unit-docker-service-not-found/12733) In order to fix it, and finally be able to use the commands, we need to tell the Docker Desktop to "attach" itself to our distro also
-In order to enable SystemD on WSL2, we will apply the scripts from [Daniel Llewellyn]([https://forum.snapcraft.io/t/running-snaps-on-wsl2-insiders-only-for-now/13033). The full blog post walks us through how he came to the solution, and the various iterations he did to fix several issues. Do watch this [video](https://www.youtube.com/watch?v=cWlYe0CE2iU) for a quick insight!