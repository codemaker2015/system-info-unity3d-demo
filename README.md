# System Information Unity3D Demo

![demo](Demos/Screenshot1.jpg)


## Source code

```cs
using System.Collections;
using System.Collections.Generic;
using UnityEngine;
using UnityEngine.UI;

public class SystemInfoScript : MonoBehaviour
{
    [SerializeField]
    Text info;
    string infoString = "";
    // Start is called before the first frame update
    void Start()
    {
       infoString += "Battery Level: " + SystemInfo.batteryLevel + "\n";
       infoString += "Battery Status: " + SystemInfo.batteryStatus + "\n";
       infoString += "Device Model: " + SystemInfo.deviceModel + "\n";
       infoString += "Device Name: " + SystemInfo.deviceName + "\n";
       infoString += "Device Type: " + SystemInfo.deviceType + "\n";
       infoString += "Device Unique Identifier: " + SystemInfo.deviceUniqueIdentifier + "\n";
       infoString += "Operating System: " + SystemInfo.operatingSystem + "\n";
       infoString += "Processor Type: " + SystemInfo.processorType + "\n";
       infoString += "Memory Size: " + SystemInfo.systemMemorySize + "\n";
       infoString += "Acceleromer Support: " + SystemInfo.supportsAccelerometer + "\n";
       infoString += "Gyroscope Support: " + SystemInfo.supportsGyroscope + "\n";
       infoString += "Vibration Support: " + SystemInfo.supportsVibration + "\n";
       info.text = infoString;

       // For more: https://docs.unity3d.com/ScriptReference/SystemInfo.html
    }

    // Update is called once per frame
    void Update()
    {
        
    }
}
```

For more: https://docs.unity3d.com/ScriptReference/SystemInfo.html