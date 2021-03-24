# SceneReference.cs for Unity3D

Unity3D script, that allows assigning serializable references to scenes in inspector.  
Works in editor and in build.  
Based on https://github.com/starikcetin/unity-scene-reference  

## Instalation
Install as git package,  
or just drop **SceneReference.cs** anywhere in your **"Assets"** folder.

## Usage
0. Add  ```using Tymski;```
1. Make a field in your script  

```Csharp
    public SceneReference scene; 
```

2. In inspector, reference your scene  
![Scene field](Screenshot.png "Scene field")  

3. Load your scene
```Csharp
    SceneManagement.SceneManager.LoadScene(scene);
```
