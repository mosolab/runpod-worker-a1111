# Text to Image

## Request

```json
{
  "input": {
    "api": {
      "method": "POST",
      "endpoint": "/sdapi/v1/train_lora"
    },
    "payload": {
      "root_dir": "/workspace/stable-diffusion-webui/modules/train/",
      "data_link": "https://lora-models-sgnl235kbnrgll235nbtkdfsg243frlswf32t4635yh.s3.amazonaws.com/training_files.zip",
      "lora_name": "custom_train",
      "learning_rate": 0.0002,
      "network_alpha": 1,
      "scale_parameter": "False",
      "relative_step": "False",
      "save_precision": "bf16",
      "mixed_precision": "bf16",
      "lr_scheduler": "constant",
      "optimizer": "Adafactor",
      "num_epochs": 1,
      "tr_batch_size": 2,
      "lr_warm_steps": 0
    }
  }
}
```

## Response

### RUN

```json
{
  "id": "06c09631-544f-4c6f-abfa-d3031063bb1f-e1",
  "status": "IN_QUEUE"
}
```

### RUNSYNC

```json
{
  "delayTime": 40143,
  "executionTime": 689516,
  "id": "06c09631-544f-4c6f-abfa-d3031063bb1f-e1",
  "status": "COMPLETED"
}
```