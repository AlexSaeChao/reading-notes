# Reading 41

## Amazon Pinpoint (we are using this for analytics)

What are three use cases for Amazon Pinpoint?

> - **Send one-time passwords securely:** Deliver SMS or email messages to help users quickly and more easily access their accounts through secure one-time passwords with unique login codes.
> - **Engage with users in real time:** Send real-time notifications to customer segments about breaking news, local updates, or event notices.
> - **Proactively surface order status changes:** Automatically inform customers when orders are picked up, in transit, or delivered to their door.

What are some analytics you think would be important to track in an application?

- **User Engagement Metrics are important:** The number of active users, session lengths, and frequency of app usage.

- **Conversion Rates:** Understanding how many users actually perform a desired action after receiving a push notification or clicking on an in-app message.

- **Retention Rates:** Measure how many users continue to use the app over time, which can help in identifying features or content that keep users engaged.

- **User Flow:** Analyzing the paths users take through the app can help identify bottlenecks or areas where users drop off.

## Amazon Polly (we are using this for text-to-speech)

In non-technical terms, what service does Amazon Polly provide?

> Amazon Polly is a cloud service that converts text into lifelike speech. It's like having a virtual reader that reads your text out loud. You could even convert that text to an MP3 some how!

What are the benefits of the Amazon Polly service?

> Some of the benefits of using Amazon Polly include:

> - **High quality** – Amazon Polly offers both new neural TTS and best-in-class standard TTS technology to synthesize the superior natural speech with high pronunciation accuracy (including abbreviations, acronym expansions, date/time interpretations, and homograph disambiguation).
> - **Low latency** – Amazon Polly ensures fast responses, which make it a viable option for low-latency use cases such as dialog systems.
> - **Support for a large portfolio of languages and voices** – Amazon Polly supports dozens of voices languages, offering male and female voice options for most languages. Neural TTS currently supports three British English voices and eight US English voices. This number will continue to increase as we bring more neural voices online. US English voices Matthew and Joanna can also use the Neural Newscaster speaking style, similar to what you might hear from a professional news anchor.
> - **Cost-effective** – Amazon Polly's pay-per-use model means there are no setup costs. You can start small and scale up as your application grows.
> - **Cloud-based solution** – On-device TTS solutions require significant computing resources, notably CPU power, RAM, and disk space. These can result in higher development costs and higher power consumption on devices such as tablets, smart phones, and so on. In contrast, TTS conversion done in the AWS Cloud dramatically reduces local resource requirements. This enables support of all the available languages and voices at the best possible quality. Moreover, speech improvements are instantly available to all end-users and do not require additional updates for devices.

## Things I want to know more about

### Amazon Polly

1. **Text Length and Complexity**:
    - Are there any limitations on the length or complexity of the text that can be converted to speech?

2. **Language, Dialect, and Accent Support**:
    - While multiple languages are supported, you may want to check if the specific dialect or accent you need is available.

3. **Intonation and Emotion**:
    - Does Polly support varied intonations or emotions to make the speech sound more natural?

### Amazon Pinpoint

1. **Integration with Non-AWS Services**:
    - How well does Pinpoint integrate with other services that are not part of AWS? Are there any special considerations or limitations?

2. **Compatibility Concerns**:
    - What should we stay away from in terms of technologies or services that may not be compatible or optimal when using Pinpoint or Polly?

## References

[Amazon Pinpoint (we are using this for analytics)](https://aws.amazon.com/pinpoint/)

[Amazon Polly (we are using this for text-to-speech)](https://docs.aws.amazon.com/polly/latest/dg/what-is.html)
