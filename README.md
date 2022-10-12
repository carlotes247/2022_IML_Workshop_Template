# 2022_IML_Workshop_Template
InteractML template project with XR support for 2022 workshops

## Installation 
```
# clone project
git clone https://github.com/carlotes247/2022_IML_Workshop_Template.git

# go to your newly created project folder
cd 2022_IML_Workshop_Template

# add InteractML as a submodule
git submodule add -b VRInterface --force https://github.com/Interactml/iml-unity.git Assets/iml-unity

# add InteractML_Telemetry as a submodule 
git submodule add https://github.com/carlotes247/InteractML_Telemetry.git Assets/iml-unity-telemetry

# navigate and clean broken files from iml-unity submodule
cd Assets/iml-unity
git sparse-checkout init --cone
git sparse-checkout set Assets

# done :)
```
