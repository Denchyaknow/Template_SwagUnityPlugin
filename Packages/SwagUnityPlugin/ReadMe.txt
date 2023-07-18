//Here is an Example Package Manifest

Use the displayName property to give your package a user-friendly name that appears in the Package Manager window and other places in the Unity Editor. For example, “My Custom Plugin”.
Use the description property to give your package a brief description that appears in the details view of the Package Manager window. You can use UTF-8 character codes to format your text, such as line breaks (\n) and bullets (\u25AA).
Use the unity property to indicate the lowest Unity version that your package is compatible with. This helps users to avoid installing incompatible packages for their projects.
Use the dependencies property to list the other packages that your package depends on. You can specify the minimum version required for each dependency using semantic versioning. For example, "com.unity.modules.ui": "1.0.0".
Use the repository property to provide a Git URL for your package source code. This helps users to find and contribute to your package if they want to. You can also specify a subdirectory or a revision using the extended syntax. For example, "repository": {"type": "git","url": "https://github.com/mycompany/myassetrepo.git?path=/Packages/MyCustomPlugin#1.0.0"}.
Use the keywords property to add some tags that describe your package and make it easier to find by users. For example, "keywords": ["plugin", "awesome", "tool"].
Use the author property to provide some information about yourself or your company, such as name, email, and URL. For example, "author": {"name": "My Company","email": "contact@mycompany.com","url": "https://mycompany.com"}.

{ 
    “name”: “com.mycompany.mycustomplugin”, 
    “version”: “1.0.0”, 
    “displayName”: “My Custom Plugin”, 
    “description”: “A plugin that does something awesome”, 
    “dependencies”: 
    { 
        “com.unity.modules.ui”: 
        “1.0.0” 
    }, 
    “repository”: 
    { 
        “type”: “git”, 
        “url”: “https://github.com/mycompany/myassetrepo.git?path=/Packages/MyCustomPlugin” 
    } 
}