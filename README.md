# BytePS Examples

This repo contains several examples to run BytePS, including popular CV/NLP models implemented in TensorFlow/PyTorch/MXNet.


## Usage

A `run.sh` is provided for each example to demonstrate the basic usage. It does not set up the necessary enviroment variables needed by BytePS. Therefore, before you run these examples, we recommend you read [this tutorial](https://github.com/bytedance/byteps/blob/master/docs/step-by-step-tutorial.md) for detailed guidelines on launching BytePS. Usually it will be easier to get started on a simple example with small number of GPUs.

We also provide options to switch to Horovod for performance comparison. To do so, you should change `bpslaunch` to MPI-based command (see [Horovod tutorial](https://github.com/horovod/horovod#running-horovod)), and then change the value of related environment variable (usually `DISTRIBUTED_FRAMEWORK`) or python trailing argument as noted in each `run.sh`.

## Acknowledgement

Some of our examples rely on public repos, including:
- https://github.com/tensorflow/models
- https://github.com/dmlc/gluon-nlp
- https://github.com/huggingface/transformers
- https://github.com/znxlwm/UGATIT-pytorch

We use most of their code while slightly modify the communication part in order to use BytePS. 