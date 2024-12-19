This app is used for cropping orthophotos, preparing them for training to generate a pre-trained model.

The reason for adding the environment is because changes were made to the file 
```bash
"Crop-Merge\env\Lib\site-packages\PIL\Image.py".
```

From this:
```bash
MAX_IMAGE_PIXELS: int | None = int(1024 * 1024 * 1024 // 4 // 3)
```

To this:
```bash
MAX_IMAGE_PIXELS: int | None = None
```

You can either install your own environment or use this one.

Make sure to have the following Python version. You can check it in the file 
```bash
"Crop-Merge\env\pyvenv.cfg"
 ```
