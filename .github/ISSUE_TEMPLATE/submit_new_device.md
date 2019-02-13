---
title: 'Your device name and model'
labels: new device
assignees: T-vK
---

If you found a new device, then please use the following JSON and delete the data from it, then insert as much data about your device as you can.  
Thanks you. :)  

``` JSON
{
    "name": "Razer Blade 15 (2018 Basic)",
    "cpu": "Intel Core i7-8750H",
    "gpus": [
        {
            "name": "GTX 1060 Mobile with Max-Q design (6GB)",
            "type": "dGPU",
            "passthrough-guests": {
                "Windows": "Works, but Nvidia driver fails with error 43.",
                "Linux": "Untested, but probably works."
            }
        },
        {
            "name": "Intel® UHD Graphics 630",
            "type": "iGPU",
            "passthrough-guests": {
                "Windows": "Untested, but probably works.",
                "Linux": "Untested, but probably works."
            }
        },
        {
            "name": "GTX 970",
            "type": "eGPU",
            "passthrough-guests": {
                "Windows": "Works, but Nvidia driver fails with error 43.",
                "Linux": "Untested, but probably works."
            }
        }
    ],
    "checklist": {
        "linux-compatible": "Yes, no issues",
        "at-least-two-usable-gpus": "Yes",
        "cpu-supports-iommu": "Yes",
        "chipset-supports-iommu": "Yes",
        "uefi-supports-iommu": "Yes",
        "igpu-usable": "Yes",
        "muxed": "Probably yes"
    },
    "tested-by": [
        { "name": "T-vK", "url": "https://github.com/T-vK" }
    ],
    "notes": "Supports TB3 eGPUs"
}
```

If anything is unclear, feel free to ask!  
Instead of opening this issue, you can also simply fork this project, add your JSON to the notebook-compatibility-list.json and submit your changes as a Pull-Request.
