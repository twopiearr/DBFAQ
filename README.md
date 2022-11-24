**Q: Where does Diffusion Bee keep it's models/images/other support files?**
*A: In a hidden directory in your User directory called .diffusionbee. The easiest way to expose it is to open a Terminal window and type `open ~/.diffusionbee` and hit Return; you can close the Terminal window once you're done. If you want more details, google "Mac OS X hidden directories". 

**Q: What model does Diffusion Bee use?**

A: Diffusion Bee is currently available in a "low quality" FP16 version that uses the MPS backend, and a "high quality" FP32 version that uses the TensorFlow backend. The "low quality" version uses the 1.5 model, the "high quality" version uses the 1.4 model. You can load custom models into either version.

**Q: How do I load a new model into Diffusion Bee?**

A: From the hamburger menu in the upper right corner, select Settings. From that screen you should find a button to import a new model. Once you have imported the model, Diffusion Bee has no more use for the .ckpt file, so you can delete it or archive it as you see fit.

Q: I tried that, but it gave me an error instead of loading the model. What do I do?
A: At this time there are a few models known to not load. Notably among these is the Novel-AI anime model, for which no support is expected, and the Waifu FP32 model, which should be fixed in the next release (the 16FP model works fine). There is a bug fix that has been merged into the code and should exist in the next version (past 1.5.1) that should address this issue. 

Q: How do I use a new model once I've loaded it into Diffusion Bee?
A: As of version 1.5.1 of Diffusion Bee, the Options window has a button that allows you to choose one of the models you've loaded.

Q: I did that, but I'm not getting the output I expect.
A: Most Dreambooth models have a specific token you need to use to activate the effect. Go back the source from where you got the model and look at the ReadMe file, or other documentation. The trigger token should be listed. 

Q: I used the trigger token, and I'm still getting garbage output.
A: There is a known issue with importing a few models (such as PaperCut). There is a bug fix that has been merged into the code and should exist in the next version (past 1.5.1) that should address this issue.

Q: What model is used for Inpainting/Outpainting?
A: The Runway 1.5 inpainting model.

Q: How can I specify a different model for Inpainting/Outpainting?
A: At this time, you can't.

Q: I don't see the Import Model button in the Settings window.
A: You are not using the latest version of Diffusion Bee. Download it from here: https://github.com/divamgupta/diffusionbee-stable-diffusion-ui/releases

Q: What sampler does Diffusion Bee use?
A: Based on notes we'e seen in the code, we believe it is using the DDIM sampler.

Q: How do I change the sampler?
A: At this time you cannot.

Q: Will the next version of Diffusion Bee use the new 2.0 model?
A: No announcement has been made at this time.

Q:Can this version of Diffusion Bee import the 2.0 model?
A: Stability AI (the company that released it) has confirmed that code base modifications are necessary for ANY implementation to use the 2.0 model. Until those modifications are incorporated into Diffusion Bee, the 2.0 model cannot be supported. This is true of every implementation that exists.
