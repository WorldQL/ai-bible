
## Variations of models
There are several different versions of Stable Diffusion which have compatibility issues with one-another.
- Stable Diffusion 1.5 is the most popular version and was trained on a diverse set of images. It has the largest range and most community fine-tunes.
- Stable Diffusion 2.0. Relatively unpopular. Notably has the depth diffusion model variant.
- Stable Diffusion 2.1.

## Fine Tuning Stable Diffusion
There are a variety of techniques for further controlling the output:
- [[Naive fine-tuning]]
	- Adds information to the model
	- Causes the output to match the input dataset more closely.
- [[Dreambooth]]
	- Adds information to the model. Produces checkpoints which are the same size as a full stable diffusion model (5GB+)
	- Useful for creating multiple images of a consistent subject.
	- Uses a class (the type of the subject, usually "a picture of an artbible123 person") and a token that doesn't conflict with any existing tokens ("artbible123")
- [[LoRA]]
	- Low rank adaption, adds information to the model. Usually less than 50MB.
	- Can be used for the same purposes as a Dreambooth finetune.
- Textual inversion
	- Creates a new token that's associated with a certain subject's location in latent space. Does not add new information to the model. Usually only a few KB.
	- Requires only 5-10 images of the concept you want to train.
- Hypernetwork
	- Used to fine-tune style and "post processing" finishes. Can sometimes learn new subjects.
- [[VAEs]]
	- Variational autoencoders. Used for fine-tuning final details
- [[Samplers or CLIP Guidance]]

## Obtaining Models
https://rentry.org/sdmodels#stable-diffusion-v20
https://civitai.com/