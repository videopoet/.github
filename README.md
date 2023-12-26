# VideoPoet is Google's A large language model for zero-shot video generation

a simple modeling method that can convert any autoregressive language model or large language model (LLM) into a high-quality video generator. 

It contains a few simple components:

 - A pre-trained MAGVIT V2 video tokenizer and a SoundStream audio tokenizer transform images, video, and audio clips with variable lengths into a sequence of discrete codes in a unified vocabulary. These codes are compatible with text-based language models, facilitating an integration with other modalities, such as text.

 - An autoregressive language model learns across video, image, audio, and text modalities to autoregressively predict the next video or audio token in the sequence.

 - A mixture of multimodal generative learning objectives are introduced into the LLM training framework, including text-to-video, text-to-image, image-to-video, video frame continuation, video inpainting and outpainting, video stylization, and video-to-audio. Furthermore, such tasks can be composed together for additional zero-shot capabilities (e.g., text-to-audio).

This simple recipe shows that language models can synthesize and edit videos with a high degree of temporal consistency. VideoPoet demonstrates state-of-the-art video generation, in particular in producing a wide range of large, interesting, and high-fidelity motions. The VideoPoet model supports generating videos in square orientation, or portrait to tailor generations towards short-form content, as well as supporting audio generation from a video input.

[Click to Video](https://storage.googleapis.com/googwebreview.appspot.com/grow-ext-cloud-images-uploads/2z73455wyhhm-1mtsV1LWXSHTiEABiYXKQx-08df0dcc93bdb403ca30f844d0a927e9-videopoet_header_video_35F06F4F.mp4)

# Authors

Dan Kondratyuk*, Lijun Yu*, Xiuye Gu*, José Lezama*, Jonathan Huang, Rachel Hornung, Hartwig Adam, Hassan Akbari, Yair Alon, Vighnesh Birodkar, Yong Cheng, Ming-Chang Chiu, Josh Dillon, Irfan Essa, Agrim Gupta, Meera Hahn, Anja Hauth, David Hendon, Alonso Martinez, David Minnen, David Ross, Grant Schindler, Mikhail Sirotenko, Kihyuk Sohn, Krishna Somandepalli, Huisheng Wang, Jimmy Yan, Ming-Hsuan Yang, Xuan Yang, Bryan Seybold*, Lu Jiang*

*Equal technical contribution

[Offfical Website](https://sites.research.google/videopoet/)
