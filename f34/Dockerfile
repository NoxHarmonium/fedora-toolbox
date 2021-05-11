FROM registry.fedoraproject.org/f34/fedora-toolbox:34

# Setup VSCode repo
RUN sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc && sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'

# Install common dependencies
RUN sudo dnf install -y glibc-all-langpacks direnv fish neovim git-delta libX11-xcb libdrm fira-code-fonts code && dnf clean all 

