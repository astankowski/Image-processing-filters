# Image-processing-filters
## How to run

Use make in project's directory

```bash
  make
```

```bash
  ./point -h
  Usage: point [-h] -i <input> -o <output> -f <filter> [-t <times>] [-a <axis>] [-p <percent>]
  -i, --input-file=<input>  Input JPEG File
  -o, --out-file=<output>   Output JPEG File
  -f, --filter=<filter>     Filter
  -t, --times=<times>       Multiplyer
  -h, --help                print this help and exit
  -a, --axis=<axis>         Axis for flip (x/y)
  -p, --percent=<percent>   Change percent
```

## Usage examples
![sample_image](https://github.com/user-attachments/assets/dd0d0273-a494-431d-8641-993d37730730)
### Negative filter
```bash
  ./point -i sample_image.jpeg -o sample_image_negate.jpeg -f negate
```
![sample_image_negate](https://github.com/user-attachments/assets/2faf4b1b-d8b3-4ea0-96ea-1847abd22d8e)
### Brightness filter
```bash
  ./point -i sample_image.jpeg -o sample_image_brightness.jpeg -f brightness -p 100
```
![sample_image_brightness](https://github.com/user-attachments/assets/af986769-fe6c-4483-8687-c277ddb6c596)

### Contrast filter
```bash
  ./point -i sample_image.jpeg -o sample_image_contrast.jpeg -f contrast -t 2
```
![sample_image_contrast](https://github.com/user-attachments/assets/37897520-c316-4b45-acee-f81a916edac2)

### Flip filter
```bash
  ./point -i sample_image.jpeg -o sample_image_flip.jpeg -f flip --axis x
```
![sample_image_flip](https://github.com/user-attachments/assets/efc8fe08-afd5-4ba4-9516-614ca3d5c7ed)

### Rotate filter
```bash
  ./point -i sample_image.jpeg -o sample_image_rotate.jpeg -f rotate -d left
```
![sample_image_rotate](https://github.com/user-attachments/assets/c0ca3769-7990-451f-a3fb-3f910bfbcc6e)
