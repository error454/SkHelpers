# SkookumScript Helpers
This is a repository of various helpers that I've written for various SkookumScript projects. Many of these are simple wrappers whose only achievement is providing sane defaults so that you don't need to pass in a ton of arguments to common functions. Others add functionality that is missing in Unreal Engine 4.

# How to Install
* Clone or download this repo somewhere.
* In your project folder edit `Scripts/Skookum-project.ini` and add the path to the repo as an overlay, make sure you adjust overlay numbers appropriately. If you'd like to make changes to the code in this overlay then place it prior to your project overlay like I've done in the example below, otherwise you can put it last.

```
Overlay1=*Core|Core
Overlay2=-*Core-Sandbox|Core-Sandbox
Overlay3=*VectorMath|VectorMath
Overlay4=*Engine-Generated|Engine-Generated|A
Overlay5=*Engine|Engine
Overlay6=SkHelpers|C:\GitHub\SkHelpers
Overlay7=*Project-Generated-BP|Project-Generated-BP|C
Overlay8=*Project-Generated-C++|Project-Generated-C++|A
Overlay9=Project|Project
```

# What's Included 
## (Alphabetical by class)

### Actor

* [destroy\_sk\_actor](https://github.com/error454/SkHelpers/blob/master/Object/Entity/Actor/destroy_sk_actor().sk)
* [furthest\_in\_dir](https://github.com/error454/SkHelpers/blob/master/Object/Entity/Actor/furthest_in_dir()C.sk)

### AnimInstance

* [\_wait\_anim\_state](https://github.com/error454/SkHelpers/blob/master/Object/Entity/AnimInstance/_wait_anim_state().sk)

### Boolean

* [map](https://github.com/error454/SkHelpers/blob/master/Object/Boolean/map().sk)
* [\_wait\_cycle\_return\_value](https://github.com/error454/SkHelpers/blob/master/Object/Boolean/_wait_cycle_return_value().sk)
* [\_wait\_false\_true](https://github.com/error454/SkHelpers/blob/master/Object/Boolean/_wait_false_true().sk)
* [\_wait\_true\_false](https://github.com/error454/SkHelpers/blob/master/Object/Boolean/_wait_true_false().sk)

### CameraComponent
* [aspect\_ratio\_constrained?](https://github.com/error454/SkHelpers/blob/master/Object/Entity/ActorComponent/SceneComponent/CameraComponent/aspect_ratio_constrained-Q().sk)

### GameLib
* [deproject\_nscreen\_to\_world](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/GameLib/deproject_nscreen_to_world()C.sk)
* [deproject\_point\_to\_plane](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/GameLib/deproject_point_to_plane()C.sk)
* [viewport\_coordinates\_norm\_to\_screen](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/GameLib/viewport_coordinates_norm_to_screen()C.sk)
* [viewport\_coordinates\_screen\_to\_norm](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/GameLib/viewport_coordinates_screen_to_norm()C.sk)
* [viewport\_size](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/GameLib/viewport_size()C.sk)

### HitResult

* [!fake](https://github.com/error454/SkHelpers/blob/master/Object/UStruct/HitResult/!fake().sk)

### Integer

* [even?](https://github.com/error454/SkHelpers/blob/master/Object/Integer/even-Q().sk)
* [odd?](https://github.com/error454/SkHelpers/blob/master/Object/Integer/odd-Q().sk)

### LevelSequenceActor

* [jump\_to\_end](https://github.com/error454/SkHelpers/blob/master/Object/Entity/Actor/LevelSequenceActor/jump_to_end().sk)

### Object

* [\_wait\_frames](https://github.com/error454/SkHelpers/blob/master/Object/_wait_frames().sk)

### PlayerController

* [active\_camera](https://github.com/error454/SkHelpers/blob/master/Object/Entity/Actor/Controller/PlayerController/active_camera().sk)

### SoundCue

* [\_play](https://github.com/error454/SkHelpers/blob/master/Object/Entity/SoundBase/SoundCue/_play().sk)
* [play](https://github.com/error454/SkHelpers/blob/master/Object/Entity/SoundBase/SoundCue/play().sk)

### SystemLib

* [print\_log](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/SystemLib/print_log()C.sk)
* [print\_screen](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/SystemLib/print_screen()C.sk)

### Transform

* [near?](https://github.com/error454/SkHelpers/blob/master/Object/Transform/near-Q().sk)

### Vector3

* [!one](https://github.com/error454/SkHelpers/blob/master/Object/Vector3/!one().sk)

### World

* [\_time\_dilation\_ramp](https://github.com/error454/SkHelpers/blob/master/Object/Entity/World/_time_dilation_ramp().sk)

## Hierarchical

* Object
    * [\_wait\_frames](https://github.com/error454/SkHelpers/blob/master/Object/_wait_frames().sk)
    * Boolean
        * [map](https://github.com/error454/SkHelpers/blob/master/Object/Boolean/map().sk)
        * [\_wait\_cycle\_return\_value](https://github.com/error454/SkHelpers/blob/master/Object/Boolean/_wait_cycle_return_value().sk)
        * [\_wait\_false\_true](https://github.com/error454/SkHelpers/blob/master/Object/Boolean/_wait_false_true().sk)
        * [\_wait\_true\_false](https://github.com/error454/SkHelpers/blob/master/Object/Boolean/_wait_true_false().sk)
    * Entity
        * Actor
            * [destroy\_sk\_actor](https://github.com/error454/SkHelpers/blob/master/Object/Entity/Actor/destroy_sk_actor().sk)
            * [furthest\_in\_dir](https://github.com/error454/SkHelpers/blob/master/Object/Entity/Actor/furthest_in_dir()C.sk)
            * Controller
                * PlayerController
                    * [active\_camera](https://github.com/error454/SkHelpers/blob/master/Object/Entity/Actor/Controller/PlayerController/active_camera().sk)
            * LevelSequenceActor
                * [jump\_to\_end](https://github.com/error454/SkHelpers/blob/master/Object/Entity/Actor/LevelSequenceActor/jump_to_end().sk)
        * ActorComponent
            * SceneComponent
                * CameraComponent
                    * [aspect\_ratio\_constrained?](https://github.com/error454/SkHelpers/blob/master/Object/Entity/ActorComponent/SceneComponent/CameraComponent/aspect_ratio_constrained-Q().sk)
        * AnimInstance
            * [\_wait\_anim\_state](https://github.com/error454/SkHelpers/blob/master/Object/Entity/AnimInstance/_wait_anim_state().sk)
        * BlueprintFunctionLibrary
            * GameLib
                * [deproject\_nscreen\_to\_world](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/GameLib/deproject_nscreen_to_world()C.sk)
                * [deproject\_point\_to\_plane](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/GameLib/deproject_point_to_plane()C.sk)
                * [viewport\_coordinates\_norm\_to\_screen](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/GameLib/viewport_coordinates_norm_to_screen()C.sk)
                * [viewport\_coordinates\_screen\_to\_norm](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/GameLib/viewport_coordinates_screen_to_norm()C.sk)
                * [viewport\_size](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/GameLib/viewport_size()C.sk)
            * SystemLib
                * [print\_log](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/SystemLib/print_log()C.sk)
                * [print\_screen](https://github.com/error454/SkHelpers/blob/master/Object/Entity/BlueprintFunctionLibrary/SystemLib/print_screen()C.sk)
        * SoundBase
            * SoundCue
                * [\_play](https://github.com/error454/SkHelpers/blob/master/Object/Entity/SoundBase/SoundCue/_play().sk)
                * [play](https://github.com/error454/SkHelpers/blob/master/Object/Entity/SoundBase/SoundCue/play().sk)
        * World
            * [\_time\_dilation\_ramp](https://github.com/error454/SkHelpers/blob/master/Object/Entity/World/_time_dilation_ramp().sk)
    * Integer
        * [even?](https://github.com/error454/SkHelpers/blob/master/Object/Integer/even-Q().sk)
        * [odd?](https://github.com/error454/SkHelpers/blob/master/Object/Integer/odd-Q().sk)
    * UStruct
        * HitResult
            * [!fake](https://github.com/error454/SkHelpers/blob/master/Object/UStruct/HitResult/!fake().sk)
    * Transform
        * [near?](https://github.com/error454/SkHelpers/blob/master/Object/Transform/near-Q().sk)
    * Vector3
        * [!one](https://github.com/error454/SkHelpers/blob/master/Object/Vector3/!one().sk)
