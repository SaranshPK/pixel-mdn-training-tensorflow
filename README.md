# pixel-mdn-training-tensorflow
 
Required:
Python 3.6
tensorflow 2.1.0
keras 2.3.1


Setup with:
conda create --name=MDNtraining_TF python=3.6 numpy scipy matplotlib h5py jupyter tensorflow==2.1.0 keras==2.3.1


Command line prompt to run MDN_train:
python train-MDN.py --training_input INPUT_FILE.h5 --training_output OUTPUT_DIR --outFile OUTPUT_FILE_NAME --network_type NETWORK_TYPE --config CONFIG.json

NETWORK_TYPE options : 'number','pos1','pos2','pos3', 'error1x', 'error1y', 'error2x', 'error2y', 'error3x', 'error3y'
CONFIG.json is generated by genconfig.py with the same NETWORK_TYPE options as its sole parameter

Command line prompt to run genconfig:
python genconfig.py --type NETWORK_TYPE > CONFIG.json
