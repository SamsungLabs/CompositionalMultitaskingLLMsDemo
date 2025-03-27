# On-device Demonstration of Compositional Multi-tasking in Large Language Models

We provide a downloadable installable package to support our on-device demo showing compositional multi-tasking in large language models (LLMs). More specifically, we demonstrate how we can perform the combination of summarization and translation, where we provide a short summary in Spanish for a long conversation that is in English.

From the [Releases](https://github.com/SamsungLabs/CompositionalMultitaskingLLMsDemo/releases) section, the app can be downloaded as an APK, together with the model weights provided as a ZIP file (includes both quantized LLM and adapters).

## Installation

Perform the following steps on the phone to install the app:
* Place `CompositionalMultitaskingLLMsDemo.apk` and `models.zip` files into the `Downloads` directory on the phone.
* Extract the `models.zip` file within the `Downloads` directory.
* Run `CompositionalMultitaskingLLMsDemo.apk` to install the app `personalizedLLM`. The settings of the phone may need to be adjusted to allow installation from unknown sources.
* Give permission for the `personalizedLLM` app to access files on the phone. This can be done e.g. via `Settings > Apps > Menu (3 dots) > Permission manager > Files and media > See more apps that can
access all files > personalizedLLM` (details vary according to the phone).

After these steps, the app should be ready to use. You can then click on the `personalizedLLM` app icon to open it.

We tested the demo on Samsung S23+ phone (8GB RAM), with Android 13. The app is likely to work also on phones from other brands, other Android versions and with less RAM (potentially at least 6GB).

## Usage

Note that it takes around 3-5 minutes to load the model and adapters, so a loading screen will be shown until then. Afterwards, you can use the different functions that the app provides. You can select the mode (`Zero-shot`, `Two-step LoRA` and `Merged LoRA` (ours)) and then get a random conversation (from SAMSum dataset) to try out compositional multi-tasking. In general it takes around 20 seconds to get the summary, but it depends on the approach selected. You can also input your own conversation by typing it - at least three messages are needed.

