Public key cryptography in your browser!
========================================

Thanks to [Web Cryptography][] API, you can use private key crypto right in your browser.

This set of pages lets you exchange private information with your friend using encrypted messages using only public channels
(like, agreeing on meeting in some place on IRC).
Codewise, this is mostly a compilation of few first examples from [webcrypto examples repo][].

[Web Cryptography]: https://caniuse.com/#feat=cryptography
[webcrypto examples repo]: https://github.com/diafygi/webcrypto-examples/



To SEND message to someone
--------------------------

1. Ask them to:
   - open <generate.html>
   - click "Generate" button
   - save private key (red area) for step 6
   - send you the public key (green area)

2. Open <encrypt.html>

3. Paste the public key into green area

4. Enter your message into yellow box

5. Click "Encrypt" button

6. Send the encrypted message (blue area) to recipient and ask them to:
   - open <decrypt.html>
   - paste private key from step 1 into red area
   - paste encrypted message into blue area
   - click "Decrypt" button



To RECEIVE message from someone
-------------------------------

1. Open <generate.html>

2. Click "Generate" button

3. Save private key (red area) for step 6 (or, just keep this page open)

4. Send the public key (green area) to sender and ask them to:
   - open <encrypt.html>
   - paste the public key into green area
   - enter the message into yellow box
   - click "Encrypt" button
   - send you the encrypted message (blue area)

5. Open <decrypt.html>

6. Paste private key from step 3 into red area

7. Paste encrypted message into blue area

8. Click "Decrypt" button
