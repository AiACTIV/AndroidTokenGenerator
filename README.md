# AndroidTokenGenerator

## Setup instruction
1. **Add local maven repositories into project**

   ```
   repositories {
       mavenCentral()
   }
   ```
   
2. **Add implementation for this sdk**
```
   dependencies {
     implementation 'io.aiactiv:TokenGenerator:1.0'
   }
```

3. **Usage**:

  ```
  AiTokenGenerator.genToken(this, object : AiTokenGenerator.AiTokenCallback {
            override fun onTokenGenerated(token: String?) {
            }

            override fun onError(errorMessage: String?) {
            }
        })
  ```
