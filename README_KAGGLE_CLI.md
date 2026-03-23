https://github.com/Kaggle/kaggle-cli/blob/main/docs/kernels.md#kaggle-kernels-push

Accelerators available as of Feb 2026:

    NvidiaTeslaP100
    TpuV38
    NvidiaTeslaT4
    NvidiaTeslaT4Highmem
    Tpu1VmV38
    NvidiaTeslaA100
    NvidiaL4
    TpuV5E8
    NvidiaL4X1
    TpuV6E8
    NvidiaH100
    NvidiaRtxPro6000

Some of these are only available to participants of specific competitions, and some are only available to Kaggle admins.

# Most common — request any GPU
kaggle kernels push -p ./my-notebook --accelerator gpu

# Request TPU
kaggle kernels push -p ./my-tpu-script --accelerator TpuV5E8

# Request high-end GPU (if your competition/code needs it)
kaggle kernels push -p ./big-model-training --accelerator NvidiaTeslaT4
