# NFC Deployment Notes

`NTAG215` stores only a URL, not the HTML itself.

Recommended flow:

1. Upload [`nfc-site/index.html`](/Users/yunjihyeong/Desktop/WEMD_Operator/nfc-site/index.html) to a static host.
2. Get the public `https://...` URL.
3. Write that URL to the `NTAG215` as a standard NFC URL record.

Notes:

- `NTAG215` user memory is about `504 bytes`, so a full webpage will not fit on the tag.
- Keep the final URL short if possible.
- If you use GitHub Pages, `.nojekyll` is already included in [`nfc-site/.nojekyll`](/Users/yunjihyeong/Desktop/WEMD_Operator/nfc-site/.nojekyll).
