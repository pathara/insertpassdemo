AsiaPay Voice Pay + Gift Bar Draw Demo — Version 8.4

Files
- voice-pay.html: tap intro_draft.png to enter the fixed single-screen Voice Pay experience. Gift draw is performed on the ABCDE Gift Bar after demo payment confirmation.
- voice-pay-dashboard.html: manage gift names, prices, images and Show Image settings for A–E.
- asset/: PayDollar logo, intro image, gift images and payment method logos.

Kiosk layout
- Designed for portrait 9:16, 1080 x 1920 pixels.
- Main interface stays on one screen and does not use page scrolling. The only opening transition is tapping the intro image.
- Three zones: PayDollar + Voice Pay header, Gift Bar (without a “Your Gift Bar” heading), Voice Pay payment panel.

Demo flow
1. Tap the intro image.
2. Gift Bar cycles through letters A–E while waiting for payment method selection.
3. The microphone animates as soon as the main screen opens. Select a payment method by clicking its logo or speak the payment method (browser SpeechRecognition support required).
4. Confirm using YES, CONFIRM or NO, TRY AGAIN.
5. On confirmation, the demo displays HK$0.00 / Payment Completed / Paid with ... for 3 seconds. After the 3-second payment-complete pause, a large visible 3–2–1 countdown appears without cycling/highlighting the A–E tiles. Then only the actual gift images (without names or prices) slowly fade in while the highlight speeds up for about 2 seconds, then gradually slows to the selected gift. The winning tile holds for 2 seconds before a 3-second prize pop-up and Congratulations.
6. Congratulations contains only the heading, gift image, gift name, About Voice Pay, and Play Again buttons. About Voice Pay returns to Intro; Play Again returns to payment selection.

Important
- This is a front-end demo only. No real payment is processed.
- Voice input depends on browser support and microphone permission; payment-logo click is the fallback.
- Dashboard changes are saved in localStorage for the same browser/device. Custom image uploads are stored in that browser.
- The gift draw result is randomly selected in the browser and is not a production-grade prize-control system.

Version 8.4 updates
- Removed the three rounds of A–E highlighting during countdown; a large 3–2–1 countdown is displayed instead.
- After stopping on the actual winner, the highlighted tile holds for 2 seconds before the prize pop-up.
- Congratulations content is vertically centered; the gift name is directly below Congratulations and above the image.
- Payment confirmation layout has more spacing, especially between payment-logo rows.
- Removed the PAYMENT COMPLETE kicker; HK$0.00 and Payment Completed are larger and positioned higher, with a larger Paid with line.
