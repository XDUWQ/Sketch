## Command-line Arguments

- `--train` : run network training pass (default: False)
- `--test` : run testing pass - predict maps from input sketches (default: False) 
- `--encode` : run feature encoding pass - extract features from input sketches (default: False)
- `--predict_normal` : if True, predict both depth and normal information; if False, predict depth only (default: True) 
- `--continuous_view` : if True, use a modified network architecture of Tatarchenko et al. with continuous viewing parameters as input (default: False)
- `--no_adversarial` : if True, skip adversarial loss term (default: False)
- `--batch_size INT` : use 2 for GPU with 12GB memory; use 4 for GPU with 24GB memory; the effective batch size is always 40 (default: 2)   
- `--image_size INT` : image size of input sketches and output maps (default: 256) 
- `--sketch_variations INT` : number of sketch style variations for training (default: 4)
- `--sketch_views STRING` : a string consist of one or more characters from 'F' (front), 'S' (side), 'T' (top) denoting the views of the input sketches (default: FS)  
- `--max_epochs FLOAT` : maximum number of epochs for training (default: 100)
- `--gpu_fraction FLOAT` : maximum fraction of GPU memory used (default: 0.9) 
- `--data_dir STRING` : path to the dataset directory
- `--train_dir STRING` : path to the training checkpoints & network parameters files directory 
- `--test_dir STRING` : path to the testing results output directory
- `--encode_dir STRING` : path to the encoding feature output directory
- `--view_file STRING` : an `off` format mesh file encoding output camera positions in vertex information

