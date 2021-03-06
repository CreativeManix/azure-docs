---
title: Sample for Intent Recognition | Microsoft Docs
titleSuffix: "Microsoft Cognitive Services"
description: Here is a sample for intent recognition.
services: cognitive-services
author: wolfma61
manager: onano

ms.service: cognitive-services
ms.technology: Speech
ms.topic: article
ms.date: 05/07/2018
ms.author: wolfma
---

# Sample for Intent Recognition

> [!NOTE]
> For instructions to download this sample and others, see [Samples for Speech SDK](samples.md).

> [!NOTE]
> Please obtain a subscription key first. In contrast to other services supported by the Cognitive Service Speech SDK, the Intent Recognition services requires a specific subscribtion key. [Here](https://www.luis.ai) you can find additional information about the intent recognition technology, as well as information on how to acquire a subscription key. Replace your own subscription key, the region of the service, as well as the AppId of your intent model in the appropriate place in the samples.

> [!NOTE]
> For all samples below the following top-level declarations should be in place:
>
> [!code-cpp[](~/samples-cognitive-services-speech-sdk/Windows/cxx_samples/intent_recognition_samples.cpp#toplevel)]
>
> - - -

## Intent Recognition Using Microphone

The code snippet below shows how to recognize intent from microphone input in the default language (`en-US`).

[!code-cpp[Intent Recognition Using Microphone](~/samples-cognitive-services-speech-sdk/Windows/cxx_samples/intent_recognition_samples.cpp#IntentRecognitionWithMicrophone)]

- - -

## Intent Recognition Using Microphone In a Specified Language

The code snippet below shows how to recognize intent from microphone input in a specified language, in this case in German (`de-de`).

[!code-cpp[Intent Recognition Using Microphone In A Specified Language](~/samples-cognitive-services-speech-sdk/Windows/cxx_samples/intent_recognition_samples.cpp#IntentRecognitionWithLanguage)]

- - -

## Intent Recognition From a File

The following code snippet recognizes intent from an audio file in the default language (`en-US`), the supported format is single-channel (mono) WAV / PCM with a sampling rate of 16 KHz.

[!include[Sample Audio](includes/sample-audio.md)]

[!code-cpp[Intent Recognition From a File](~/samples-cognitive-services-speech-sdk/Windows/cxx_samples/intent_recognition_samples.cpp?IntentRecognitionWithFile)]

- - -

## Intent Recognition Using Events

The code snippet shows how to recognize intent in a continuous way. This code allows access to additional information, like intermediate results. 

[!code-cpp[Intent Recognition Using Events](~/samples-cognitive-services-speech-sdk/Windows/cxx_samples/intent_recognition_samples.cpp#IntentContinuousRecognitionUsingEvents)]

- - -

## Sample Source Code

The latest version of the samples and even more advanced samples are in a dedicated [GitHub repository](https://github.com/Azure-Samples/cognitive-services-speech-sdk).

## Next Steps

- [Speech Recognition](./speech-to-text-sample.md)

- [Translation](./translation.md)
