# 2022_IML_Workshop_Template
InteractML template project with XR support for 2022 workshops

## Installation with submodules
```
# clone the project in your computer
git clone https://github.com/carlotes247/2022_IML_Workshop_Template.git

# make sure longpaths are allowed in the git console
git config --global core.longpaths true

# go to the Unity project folder where you downloaded the project
cd [your_project_folder]

# add [InteractML](https://github.com/Interactml/iml-unity) as a submodule 
git submodule add -b VRInterface --force https://github.com/Interactml/iml-unity.git Assets/iml-unity

# add [InteractML_Telemetry](https://github.com/carlotes247/InteractML_Telemetry) as a submodule 
git submodule add https://github.com/carlotes247/InteractML_Telemetry.git Assets/iml-unity-telemetry

# navigate to 'Assets/iml-unity' and clean unneeded files that will break the project
cd Assets/iml-unity
git sparse-checkout init --cone
git sparse-checkout set Assets
