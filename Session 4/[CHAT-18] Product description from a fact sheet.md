# [CHAT-18] Product description from a fact sheet

## Input

Your task is to help a marketing team create a description for a retail website of a product based on a technical fact sheet that comes in JSON format.

Write a product description based on the information provided in the technical specifications below. Maximum length: 50 words.

<fact_sheet>
```
{
    "Display": "Amazon's 7-inch Paperwhite display technology with built-in front light, 300 ppi, optimized font technology, 16-level gray scale.",
    "Size": "127.5 x 176.7 x 7.8 mm",
    "Weight": "211 g. Actual size and weight may vary by configuration and manufacturing process.",
    "System Requirements": "None; fully wireless and doesn't require a computer to download content.",
    "On-Device Storage": "16 GB; holds thousands of books.",
    "Cloud Storage": "Free cloud storage for all Amazon content.",
    "Battery Life": "A single charge lasts up to twelve (12) weeks, based on half an hour of reading per day with wireless off and the light setting at 13. Battery life may vary depending on use. Audible audiobook streaming over Bluetooth will reduce battery life.",
    "Charge Time": "Fully charges in approximately 2.5 hours with a 9 W USB-C power adaptor.",
    "Wi-Fi Connectivity": "Supports 2.4 GHz and 5.0 GHz networks with support for WEP, WPA, WPA2, WPA3 and OWE security using password authentication or Wi-Fi Protected Setup (WPS). Does not support connecting to ad-hoc (or peer-to-peer) Wi-Fi networks.",
    "Accessibility Features": "VoiceView screen reader, available over Bluetooth audio, provides spoken feedback allowing you to navigate your device and read books with text-to-speech (available in English only). Kindle Paperwhite also includes the ability to have dark mode, adjust font size, font face, line spacing, and margins. Learn more about Accessibility for Kindle.",
    "Content Formats Supported": "Kindle Format 8 (AZW3), Kindle (AZW), TXT, PDF, unprotected MOBI, PRC natively; PDF, DOCX, DOC, HTML, EPUB, TXT, RTF, JPEG, GIF, PNG, BMP through conversion; Audible audio format (AAX). Learn more about supported file types for personal documents."
}
```
</fact_sheet>

## Output (Gemini)

Here's a product description for a retail website based on the provided JSON fact sheet, keeping it within 50 words:

**Experience unparalleled reading with the Kindle Paperwhite. Enjoy a crisp 300 ppi display, weeks of battery life, and thousands of books stored on-device. Lightweight and portable, it's the perfect companion for any book lover.** 

This description highlights key features like the high-resolution display, long battery life, and ample storage capacity, appealing to potential customers.

---

## Input

Your task is to display the information contained in the following fact sheet in a Markdown table.

<fact_sheet>
```
{
    "Display": "Amazon's 7-inch Paperwhite display technology with built-in front light, 300 ppi, optimized font technology, 16-level gray scale.",
    "Size": "127.5 x 176.7 x 7.8 mm",
    "Weight": "211 g. Actual size and weight may vary by configuration and manufacturing process.",
    "System Requirements": "None; fully wireless and doesn't require a computer to download content.",
    "On-Device Storage": "16 GB; holds thousands of books.",
    "Cloud Storage": "Free cloud storage for all Amazon content.",
    "Battery Life": "A single charge lasts up to twelve (12) weeks, based on half an hour of reading per day with wireless off and the light setting at 13. Battery life may vary depending on use. Audible audiobook streaming over Bluetooth will reduce battery life.",
    "Charge Time": "Fully charges in approximately 2.5 hours with a 9 W USB-C power adaptor.",
    "Wi-Fi Connectivity": "Supports 2.4 GHz and 5.0 GHz networks with support for WEP, WPA, WPA2, WPA3 and OWE security using password authentication or Wi-Fi Protected Setup (WPS). Does not support connecting to ad-hoc (or peer-to-peer) Wi-Fi networks.",
    "Accessibility Features": "VoiceView screen reader, available over Bluetooth audio, provides spoken feedback allowing you to navigate your device and read books with text-to-speech (available in English only). Kindle Paperwhite also includes the ability to have dark mode, adjust font size, font face, line spacing, and margins. Learn more about Accessibility for Kindle.",
    "Content Formats Supported": "Kindle Format 8 (AZW3), Kindle (AZW), TXT, PDF, unprotected MOBI, PRC natively; PDF, DOCX, DOC, HTML, EPUB, TXT, RTF, JPEG, GIF, PNG, BMP through conversion; Audible audio format (AAX). Learn more about supported file types for personal documents."
}
```
</fact_sheet>

## Output (Gemini)

Here's the information from the fact sheet displayed in a Markdown table:

```
Markdown

| Feature | Description |
|---|---|
| Display | Amazon's 7-inch Paperwhite display technology with built-in front light, 300 ppi, optimized font technology, 16-level gray scale. |
| Size | 127.5 x 176.7 x 7.8 mm |
| Weight | 211 g. Actual size and weight may vary by configuration and manufacturing process. |
| System Requirements | None; fully wireless and doesn't require a computer to download content. |
| On-Device Storage | 16 GB; holds thousands of books. |
| Cloud Storage | Free cloud storage for all Amazon content. |
| Battery Life | A single charge lasts up to twelve (12) weeks, based on half an hour of reading per day with wireless off and the light setting at 13. Battery life may vary depending on use. Audible audiobook streaming over Bluetooth will reduce battery life. |
| Charge Time | Fully charges in approximately 2.5 hours with a 9 W USB-C power adaptor. |
| Wi-Fi Connectivity | Supports 2.4 GHz and 5.0 GHz networks with support for WEP, WPA, WPA2, WPA3 and OWE security using password authentication or Wi-Fi Protected Setup (WPS). Does not support connecting to ad-hoc (or peer-to-peer) Wi-Fi networks. |
| Accessibility Features | VoiceView screen reader, available over Bluetooth audio, provides spoken feedback allowing you to navigate your device and read books with text-to-speech (available in English only). Kindle Paperwhite also includes the ability to have dark mode, adjust font size, font face, line spacing, and margins. Learn more about Accessibility for Kindle. |
| Content Formats Supported | Kindle Format 8 (AZW3), Kindle (AZW), TXT, PDF, unprotected MOBI, PRC natively; PDF, DOCX, DOC, HTML, EPUB, TXT, RTF, JPEG, GIF, PNG, BMP through conversion; Audible audio format (AAX). Learn more about supported file types for personal documents. |
```

This Markdown table will render neatly in many platforms, such as GitHub, GitLab, and various markdown editors.
