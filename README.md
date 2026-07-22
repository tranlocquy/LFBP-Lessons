# LFBP Lessons

Public, signed lesson downloads for the **Learn French by Podcast** iOS app.

## Distribution files

- `catalog.json` is the catalog URL consumed by the app.
- `packages/*.lfbplesson` are compressed lesson archives.
- `public-key.txt` is the Base64-encoded Ed25519 public verification key.

Every package is an AES-encrypted ZIP containing declarative lesson content,
podcast audio, word timing data, offline pronunciation clips, a canonical
manifest, and an Ed25519 signature. The iOS app decrypts packages automatically
during installation. Neither the private signing key nor the package decryption
key is stored in this public repository.

Catalog URL:

```text
https://raw.githubusercontent.com/tranlocquy/LFBP-Lessons/main/catalog.json
```
