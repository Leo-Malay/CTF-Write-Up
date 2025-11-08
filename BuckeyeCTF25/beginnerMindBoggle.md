bctf{tr1pl3_7H3_l4yeRs_Tr1pl3_thE_EncryPt10N}

1. The file is encoded in the language BrainFuck, first we decode it leading to hex data.
2. base64.b64decode(bytes.fromhex(s)).decode() use this to decode leading to the flag.
