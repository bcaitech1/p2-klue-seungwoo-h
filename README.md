# [Stage 2] Wrap-up Report

**ํ์น์ฐ T1226**

*April, 2021 - Boostcamp AI Tech*

---

## ๐ ๋ฌธ์  ์ ์์ ๋ฐ์ดํฐ์

๋๋ฒ ์งธ ๋ํ๋ ๋ฌธ์ฅ์์ ๋ ๊ฐ์ฒด ๊ฐ์ ๊ด๊ณ๋ฅผ ๋ฌธ์ฅ์ผ๋ก ๋ถํฐ ๋ฏธ๋ฆฌ ์ ์๋ 42๊ฐ (๊ด๊ณ ์์ ํฌํจ) ์ ํด๋์ค๋ก ๋ถ๋ฅ ํ๋ ๋ฌธ์  ์๋ค. ๋ํ ๊ธฐ๊ฐ์ ์ฝ 2์ฃผ ์์ผ๋ฉฐ, ์๋ฒ ํ๊ฒฝ์์ V100 GPU 1์ฅ์ ์ฌ์ฉํ์ฌ ํ์ตํ์๋ค.

- **ํ๊ฐ ์งํ**
    - Accuracy

KLUE ๋ฐ์ดํฐ์์ ์ด 9์ฒ๊ฐ์ ํ์ต ๋ฐ์ดํฐ์ 1์ฒ๊ฐ์ ํ์คํธ ๋ฐ์ดํฐ๋ก ๊ตฌ์ฑ๋์ด ์์์ผ๋ฉฐ, csv ํ์ผ ๋ด์ ๋ฌธ์ฅ, ๋๊ฐ์ entity ๊ทธ๋ฆฌ๊ณ  ๊ทธ๊ฒ๋ค์ ์ธ๋ฑ์ค ์ ๋ณด๊ฐ ๋ด๊ฒจ์ ธ ์์๋ค.

---

## ๐ ๋ฐ์ดํฐ์์ ๊ตฌ์ฑ์ ๋ฐ๋ฅธ ํ์ต ์ ๋ต

### Label ๋ถํฌ ์์๋ณด๊ธฐ

![images/download.png](images/download.png)

์ ์ฒด ํ์ต ๋ฐ์ดํฐ ๋ ์ด๋ธ ๋ถํฌ

![images/download-1.png](images/download-1.png)

์ฒซ๋ฒ์งธ entity ์ ๋ผ๋ฒจ ๋ถํฌ

![images/download-2.png](images/download-2.png)

๋๋ฒ์งธ entity ์ ๋ผ๋ฒจ ๋ถํฌ

์ฐ์ , ์ด๋ ๋์ ๊ฐ์ด ์ ์ฒด ํ์ต ๋ฐ์ดํฐ์ ๋ ์ด๋ธ ๋ถํฌ๋ฅผ ์์๋ณด๋ฉฐ ์์. ๋ฐ์ดํฐ๊ฐ ํ๊ฐ ์กด์ฌํ๋ ํด๋์ค๊ฐ ์กด์ฌํ  ๋งํผ ํด๋์ค ๋ถ๊ท ํ์ด ๊ต์ฅํ ์ฌํจ์ ์ ์ ์์๋ค. ํ์ต ๋ฐ์ดํฐ์ ํ์คํธ ๋ฐ์ดํฐ์ ๋ถํฌ๊ฐ ๋น์ทํ๋ค๋ ๊ฐ์  ์๋, ์ผ๋ถ ํด๋์ค๋ฅผ ์์  ๋ฒ๋ฆด ๊น ์๊ฐํ๋ฉฐ, ๋ช๊ฐ์ง ํด๋์ค๋ฅผ ํ์ค๋ก ์ฐ์ด ์ ์ถํด๋ณธ ๊ฒฐ๊ณผ, ๋ถํฌ๊ฐ ์๋นํ ๋ค๋ฆ์ ์ ์ ์์๋ค. ๋ฐ๋ผ์ ๊ทธ๋ฅ ๊ทธ๋๋ก 42๊ฐ์ ํด๋์ค๋ฅผ ์ ์งํ๊ธฐ๋ก ํ์๋ค.

### Entity

OIE UBS MBC NASA KT Marie ABC SPFL LVMH A KCC IOC KCC ๆถๆ ้ป็ Benedict Cumberbatch HUG UBS Bic Metallica KGET Kerrigan EXID GD&TOP FIFA MBC KAIST SBS ICAO A CBS JTWC A SBS RCA LVMH G-Dragon UN Fairies OECD โ Britney A GAP MBC KIA KT&G KBS Joy ASML GNU CNN ๅธถๅๅ SKC FIFA K A MBC A ASME d THX MBC ้ EU NBA L A Kylie MIT KBS MBC LPGA ไธญๅฎ DHC LH MBC SMAP PDH A LH MLB B BTS IBM IBM UEFA JTWC MLB SMAP Key MBC SKC KT&G A EBS SBS tvN KT Seventeen KMFDM A Deze CSIS MBN MBC B LG U SBS DeNA R.E.M. Oh! MBC MBC GS SHOP UEFA mariage KBS UNM Georg Saver Tiger A SK ใ A FDA AEK ASAYAN A CJ BBC A YTN 4-H ๆ้ Metallica EBS Pile DJ DOC Concern Worldwide B*Witched S MBC ABI Mnet SBS A GKL 45RPM CJ ENM A ClariS ABBA MOU FTA A C EVISU John II Casimir BBC EXILE NERIT ANU UBS A NASA EBS UN USL KT ๆๅ้ SBS LH AKA of CN WTO RCA EASD GS SHOP IMO CNN LIG IAEA GNU BMW OCN Taylor Swift Vaynerchuk NBC A KBS2 EG A A A MBC USCG MBC ็ซๆญฆ ไธธๅฝซ of PRASAC A NPT B Mr.Children EXID MBC Suede tvN BPA A AKA A EBS KT&G MBC ๆ็ฆ็ท KBS 

์ ํ์คํธ๋ ๊ด๊ณ๋ฅผ ์ฐพ์๋ด์ผํ  entity ๋ค ์ค, ํ๊ธ์ด ํฌํจ๋์ง ์์ entity ๋ค์ ์ถ๋ ฅํ ๊ฒ์ ์ผ๋ถ๋ค. ํ๊ธ์ด ์๋๊ฒ๊ณผ ํน์๋ฌธ์๋ฅผ ์ ์ ํด์ผ ํ๋ ๊ณ ๋ฏผ๋์ด ํ์ธํด๋ณธ ๊ฒฐ๊ณผ,  ๋ง์ ํน์๋ฌธ์์ ์์ด, ํ๋ฌธ ๋ฑ์ด ๊ด๊ณ๋ฅผ ์์ธกํด์ผํ  entity ๋ค์ ํฌํจ๋์ด ์์ด, ์ด ๋ถ๋ถ์ ๋ํ ์ ๊ฑฐ๋ฅผ ํ๋ฉด ์๋๊ฒ ๋ค๋ ๊ฒฐ์ ์ ํ์๋ค.

---

## โ๏ธ Tokenizer ๋น๊ตํ๊ธฐ

```python
# xlm-roberta-large
['โ์ฌ', '์', '์ ', 'โ์ ์', '๋น', 'โ๋ํ', '๋', 'โ21', '์ผ', 'โ"', '๊ตญ๋ฏผ', '๋ค', '๊ป', '์ ', 'โ์ด๋ฒ', 'โ์ด', '์ ', '์์', 'โ์ง์ง', '๋ถ', '์ง', 'ํ', 'โ์ ์น', '๊ถ', '์', 'โ์ด', 'ํฉ', '์ง', '์ฐ', '๊ณผ', 'โ', '๊ผผ', '์', '์ ์น', '๋ฅผ', 'โ์ฌ', 'ํ', 'ํ๊ณ ', 'โ์ง', '์ ', 'ํ', 'โ์ ์น', 'ํ๋ช', '์', 'โ๊ธธ์', 'โ์ด', '์ด', 'โ๋ฌ๋ผ', '"', '๊ณ ', 'โ๋งํ๋ค', '.']

# kykim/bert-kor-base
['์ฌ์', '##์ ', '์ ์', '##๋น', '๋ํ๋', '21์ผ', '[UNK]', '๊ตญ๋ฏผ', '##๋ค๊ป', '##์ ', '์ด๋ฒ', '์ด์ ', '##์์', '์ง์ง', '##๋ถ', '##์งํ', '์ ์น๊ถ', '##์', '์ด', '##ํฉ', '##์ง', '##์ฐ๊ณผ', '๊ผผ', '##์์ ', '##์น๋ฅผ', '์ฌํ', '##ํ๊ณ ', '์ง์ ํ', '์ ์น', '##ํ๋ช', '##์', '๊ธธ์', '์ด์ด', '๋ฌ๋ผ', '[UNK]', '๊ณ ', '๋งํ๋ค', '.']

# monologg/kobert
['โ์ฌ', '์', '์ ', 'โ์ ', '์', '๋น', 'โ๋ํ๋', 'โ21', '์ผ', 'โ"', '๊ตญ๋ฏผ', '๋ค', '๊ป', '์ ', 'โ์ด๋ฒ', 'โ์ด', '์ ', '์์', 'โ์ง์ง', '๋ถ', '์ง', 'ํ', 'โ์ ์น๊ถ', '์', 'โ์ด', 'ํฉ', '์ง', '์ฐ', '๊ณผ', 'โ', '๊ผผ', '์', '์ ์น', '๋ฅผ', 'โ์ฌํ', 'ํ๊ณ ', 'โ์ง', '์ ', 'ํ', 'โ์ ์น', 'ํ๋ช', '์', 'โ๊ธธ', '์', 'โ์ด์ด', 'โ๋ฌ๋ผ', '"', '๊ณ ', 'โ๋งํ๋ค', '.']

# monologg/koelectra-base-v3-discriminator
['์ฌ์์ ', '์ ์๋น', '๋ํ', '##๋', '21', '##์ผ', '"', '๊ตญ๋ฏผ', '##๋ค', '##๊ป', '##์ ', '์ด๋ฒ', '์ด์ ', '##์', '##์', '์ง์ง๋ถ์ง', '##ํ', '์ ์น', '##๊ถ', '##์', '์ด', '##ํฉ', '##์ง', '##์ฐ', '##๊ณผ', '๊ผผ์', '##์ ', '##์น', '##๋ฅผ', '์ฌํ', '##ํ', '##๊ณ ', '์ง์ ', '##ํ', '์ ์น', '##ํ๋ช', '##์', '๊ธธ', '##์', '์ด', '##์ด', '๋ฌ๋ผ', '"', '๊ณ ', '๋ง', '##ํ', '##๋ค', '.']

# bert-base-multilingual-cased
['์ฌ', '##์', '##์ ', '์ ', '##์', '##๋น', '๋', '##ํ', '##๋', '21์ผ', '"', '๊ตญ', '##๋ฏผ', '##๋ค', '##๊ป', '##์ ', '์ด', '##๋ฒ', '์ด', '##์ ', '##์์', '์ง', '##์ง', '##๋ถ', '##์ง', '##ํ', '์ ', '##์น', '##๊ถ', '##์', '์ด', '##ํฉ', '##์ง', '##์ฐ', '##๊ณผ', '๊ผผ', '##์', '##์ ', '##์น๋ฅผ', '์ฌ', '##ํ', '##ํ๊ณ ', '์ง', '##์ ํ', '์ ', '##์น', '##ํ', '##๋ช์', '๊ธธ', '##์', '์ด', '##์ด', '๋ฌ', '##๋ผ', '"', '๊ณ ', '๋งํ๋ค', '.']
```

![images/download-3.png](images/download-3.png)

์ ์ฒด ํ ํฐ ๋๋น UNK ํ ํฐ ๋น์จ

[UNK] ํ ํฐ์ด ๋ง์ด ๋์จ๋ค๋ฉด, ์ฑ๋ฅ์ด ์ข์ง ์์ ๊ฒ ๊ฐ์, ๊ฐ ํ ํฌ๋์ด์  ๋ณ๋ก, ํ์ต ๋ฐ์ดํฐ ์์์ ์ ์ฒด ํ ํฐ ๋๋น UNK ํ ํฐ ๋น์จ์ ํ์ธํด ๋ณด์๋ค. 0% ~ 2.5% ๋ก ํฐ ์ฑ๋ฅ์ฐจ๋ฅผ ๋ณด์ด์ง ์์๋ค. RoBERTa ์์, [UNK] ํ ํฐ์ ๋น์จ์ด 0% ๊ฐ ๋์๋ค๋๋ฐ, BPE ๊ฐ ์ฌ์ฉ๋ ํ ํฌ๋์ด์ ์ ์ฅ์ ์ด๋ผ๊ณ  ํ  ์ ์์๊ฒ ๊ฐ๋ค.

---

## ๐ข Training Pipeline

์์ฐ์ด ์ฒ๋ฆฌ ๊ณต๋ถ๋ฅผ ๋ณธ๊ฒฉ์ ์ผ๋ก ์์ํ๋ฉฐ, Huggingface ๐ค  ๋ผ์ด๋ธ๋ฌ๋ฆฌ์ ์นํด์ ธ ๋ณด๋ ค๋ ๋ธ๋ ฅ์ ๋ง์ด ํ ๊ฒ ๊ฐ๋ค. ์ฒ์ Huggingface ๋ฅผ ์ ํ์ ๋, ๋๋ฌด high-level ๋ก ๋ํ ๋์ด ์๋ ๋๋์ด ์์ง ์์ ๊ฑฐ๋ถ๊ฐ์ด ๋ค๊ธฐ๋ ํ์ง๋ง, ํ์ ์์ ๋ํ ๋ง์ด ์ฌ์ฉ๋๋ค ํ์ฌ ์ ๊ทน์ ์ผ๋ก ์ฌ์ฉํด๋ณด๊ธฐ๋ก ํ๋ค. ๋ํ ์ด ์ ๊ณต๋ฐ์ Huggingface ๋ฒ ์ด์ค๋ผ์ธ ์ฝ๋๋ฅผ ๋ง์ด ์ฐธ๊ณ ํ๋ฉฐ documentation ์ ์ฝ์ผ๋ฉฐ ํ์ํ ๋ถ๋ถ์ ์์ ํ์ฌ ์ฝ๋๋ฅผ ์์ฑํ์๋ค.

์ฌ์ฉ ํ ์๋ก ์ํ๋ ๊ธฐ๋ฅ์ ๋๋ถ๋ถ ํฌํจ๋์ด ์๊ณ  ๋งค์ฐ ๊ฐ๋จํ๊ฒ ํ์ต์ ์งํํ  ์ ์์ด ๋ณธ ๋ํ์ค์๋ ๋ชจ๋ Trainer ๋ฅผ ์ฌ์ฉํ์๋ค.

### Argparser & JSON Config

```bash
python train.py --config config1
python inference.py --config config1 --wandb_version run-.results0422_4:v0 --path /opt/ml/input/data/test/test.tsv
```

์ง๋ ๋ํ์์ ๋ค์ ๋ฒ์ argparser ๋ฅผ ์ด์ฉํ python project ๋ฅผ ์ ๊ทน์ ์ผ๋ก ์ฌ์ฉํ์๋ ์ค์ค๋ก์ ์ฝ์์ ์งํฌ ์ ์์๋ค. ์ ์ฒ๋ฆฌ๋ ์ฅฌํผํฐ ๋ธํธ๋ถ์์ ๋ฐ์ํ์ผ๋ก ๊ฒฐ๊ณผ๋ฅผ ํ์ธํด ๋ณด๋ฉฐ ์์ํ์ฌ tsv ํ์ผ์ ๋ฐ๋ก ์ ์ฅํด ์ฃผ์ด ํธ์ถํ๋ ๋ฐฉ์์ ํํ์๋ค.

ํ์ดํผ ํ๋ผ๋ฏธํฐ ๊ด๋ฆฌ๋ฅผ ํธํ๊ฒ ํ๊ธฐ ์ํด, ์ฌ๋ฌ configuration ์ json ํ์ผ์ ๋ง๋ค์ด ๋ฐ๋ก ๊ด๋ฆฌํ๋ค.

```json
{
    "train_id_name": "0422_3",
    "model_name": "xlm-roberta-large",
    "train_data_path": "/opt/ml/input/data/train/train_no_ner.tsv",
    "valid_data_path": "/opt/ml/input/data/train/valid_no_ner.tsv",
    "train_args": {
        "save_total_limit": 2,
        "save_steps": 100,
        "num_train_epochs": 100,
        "learning_rate": 1e-5,
        "per_device_train_batch_size": 32,
        "per_device_eval_batch_size": 32,
        "warmup_steps": 300,
        "weight_decay": 0.01,
        "logging_dir": "./logs",
        "logging_steps": 100,
        "evaluation_strategy": "steps",
        "eval_steps": 100,
        "dataloader_num_workers": 4,
        "label_smoothing_factor": 0.5,
        "load_best_model_at_end": "True"
    },
    "early_stopping_patience": 10
}
```

### WANDB

![images/_2021-04-23__2.38.49.png](images/_2021-04-23__2.38.49.png)

Wandb ์ญ์, ์ง๋ ๋ฒ ๋๋ค ํผ์ด์ธ์์์ ๋ง๋ ๋ถ์๊ฒ ์์(?) ์ ๋นํ์ฌ ๋ค์๋ฒ์ ๊ผญ ์ฌ์ฉํด๋ณด์๊ณ  ์๊ฐํ ํ๋ก์ ํธ ๊ด๋ฆฌํด ์ด์๋ค. ๋ชจ๋ธ ๋ํ 100๊ธฐ๊ฐ ๊น์ง ์ ์ฅํ  ์ ์๋๊ฒ ์ ๋ง ํธ๋ฆฌํ ๊ฒ ๊ฐ์๋ค. ์ฃผ๋ก best ๋ชจ๋ธ์ ์ ์ฅํ๊ณ , inference ์ wandb ์๋ฒ์์ ๋ก๋ํ์ฌ ์ฌ์ฉํ๋ ๋ฐฉ๋ฒ์ ์ฌ์ฉํ๋ค. ๋๋ถ์ ์ด๋ฒ ๋ํ์์ ์ด์ ์๋ ์ฉ๋ ๊ด๋ฆฌ์ ๋ฌธ์ ์์ ๊ณ ํต๋ฐ์ง ์์ ์ ์์๋ค.

---

## โ๏ธ ๋ฐ์ดํฐ ์ ์

> [https://github.com/machinereading/kor-re-gold](https://github.com/machinereading/kor-re-gold)

ํผ์ด์ธ์์ ํ์๋ค๊ณผ ์ฌ๋์ ์ฌ๋ผ์๋ ์์ ๋ฐ์ดํฐ์์ ์ฐ๋ฆฌ ๋ํ ํ์์ ๋ง๊ฒ ๊ฐ์ ํํธ๋ฅผ ๋๋  ์์ ํ๊ธฐ๋ก ํ๋ค.

![images/_2021-04-22__10.40.12.png](images/_2021-04-22__10.40.12.png)

๊ฐ๋จํ๊ฒ annotation tool ์ ๋ง๋ค์ด ๋ผ๋ฒจ๋ง ํจ์จ์ ๋์ฌ ๋ณด์๋ค.

![images/_2021-04-23__2.46.38.png](images/_2021-04-23__2.46.38.png)

ํ์์ ๋ฃฐ์ ์ ํด ์์

์ง์  RE ๋ผ๋ฒจ๋ง์ ์งํํด๋ณด๋, ๊ฒฐ์ฝ ์ฌ์ด ์์์ด ์๋์๋ค. ๋ฐฐ๊ฒฝ ์ง์์ ์ด์ฉํ๋ฉด ์ฝ๊ฒ ๋ ๋จ์ด๊ฐ์ ์ฐ๊ด์ฑ์ ์ ์ถํ  ์ ์์ง๋ง, ๊ทธ ๊ด๊ณ๋ฅผ ์จ์ ํ ๋ฌธ๋งฅ ์์์ ์ถ๋ก ์ด ๊ฐ๋ฅํ์ง ์ฌ๋ถ ๋ํ ํ๋จํด์ผ ํ์๋ค. ํ์ ๊ฐ์ ์์ํ ํํธ๋ฅผ ๋ชจ์ ๊ฒฐ๊ณผ์ ์ผ๋ก ์ฝ 260 ์ฌ ๊ฐ์ ๋ฐ์ดํฐ๋ฅผ ์ถ๊ฐ๋ก ์ป์ ์ ์์๋ค.

---

## ๐งฉ ์ฌ๋ฌ๊ฐ์ง ์๋๋ค

~~๋ฆฌ๋๋ณด๋์ ์ฌ๋ ธ๋ ์ ์๋ค์ ๋ชจ๋ ๊ธฐ๋กํ ์ํธ๊ฐ ๋ ์๊ฐ๋ ๋ฐ๋์.. ๋ชจ๋ธ๋ณ ๋ฆฌ๋๋ณด๋ ์ ์ ๋ณ๋ํญ์ ๋ฆฌํฌํธ์ ๊ธฐ๋กํ  ์ ์์๋ค..~~

![images/_2021-04-23__1.45.46.png](images/_2021-04-23__1.45.46.png)

### NER Tagging

๊ทธ๋ฌ๋ ๋ค๋ฅธ ๋์๋ค์ ์ฌ๋ฌ ์ธก๋ฉด์์ ์ ๋ฐฉ์ด๋์๊ณ , [CITY] ๋ญ์ผ๋ฅดํฌ [/CITY]๋ฅผ ์ ์ธํ ์ฌ๋ฌ ๋์๋ค์ [ORGANIZATION] ์ฐํฉ๊ตฐ [/ORGANIZATION]๊ณผ ๋์ผ๊ตฐ ์ฌ์ด์ ์น์ดํ ์ ํฌ ๋์ ํํ๋์๋ค.

- Pororo ๋ผ์ด๋ธ๋ฌ๋ฆฌ ์ฌ์ฉ
- ๊ด๊ณ๋ฅผ ์ฐพ์์ผ ํ๋ entity ์ ํด๋นํ๋ NER ํ๊ทธ๋ฅผ ์ป์ด ์ ๋ค์ ๋ถ์ฌ ๊ธฐ๋ก
- ~~์๋ชป ์ฌ์ฉํ ๋ถ๋ถ์ ๋ํ๊ฐ ๋๋๊ณ  ์๊ฒ๋์๋ค. Special token ์ผ๋ก ๋ฑ๋กํด์ค์ผํ๋ค๊ณ  ์๊ฐํ๋๋ฐ ์ถ๊ฐํ์ง ์๊ณ  ํ์ตํ๋ ๊ฒ์ด ์ณ์ ๋ฐฉ๋ฒ์ด๋ผ๊ณ  ํ๋ค.~~

### Entity Tagging

๊ทธ๋ฌ๋ ๋ค๋ฅธ ๋์๋ค์ ์ฌ๋ฌ ์ธก๋ฉด์์ ์ ๋ฐฉ์ด๋์๊ณ , [E2] ๋ญ์ผ๋ฅดํฌ [/E2]๋ฅผ ์ ์ธํ ์ฌ๋ฌ ๋์๋ค์ [E1] ์ฐํฉ๊ตฐ [/E1]๊ณผ ๋์ผ๊ตฐ ์ฌ์ด์ ์น์ดํ ์ ํฌ ๋์ ํํ๋์๋ค.

โ ์ ๋ ๋ฐฉ๋ฒ์, ๋ชจ๋ธ์๊ฒ ํ์ต์ ๊ด๋ จํ ์ ๋ณด๋ฅผ ์ข ๋ ์์ธํ ์ ๊ณตํ๋ค๋ฉด ํ์ต ์ฑ๋ฅ์ด ์ฌ๋ผ๊ฐ ๊ฒ์ด๋ผ๋ ์ ๊ทผ์์ ์งํํ๊ฒ ๋์๋ค.

โ ๊ฒฐ๊ณผ์ ์ผ๋ก NER, entity tagging ๋ ๋ฐฉ๋ฒ ๋ชจ๋ ์ฑ๋ฅ์ด ํฅ์๋์ง ์์๋ค. ๋ด๋ ค๊ฐ์ง๋ ์์๋ ๊ฒ์ ๋ณด๋ฉด, ๋ ๋ฐฉ๋ฒ์ด ํฌ๊ฒ ํ์ต์ ์ํฅ์ ๋ฏธ์น์ง ์์ ๊ฒ ๊ฐ๊ธฐ๋ ํ๋ค.

### Translation

- Pororo ๋ผ์ด๋ธ๋ฌ๋ฆฌ ์ฌ์ฉ
- ๋ฐ์ดํฐ ์ฆ๊ฐ์ ์ํด back translation ์ ์๋ํด ๋ณด๋ค, ์ฒ๋ฆฌ ์๊ฐ์ด ๋๋ฌด ๊ธธ์ด ์๋ํ ๋ฐฉ๋ฒ
- ํ๊ตญ์ด nlp ๋ฌธ์ ๊ฐ ์์ด์ ๊ทธ๊ฒ๋ณด๋ค ์ด๋ ค์ด ๋ฌธ์ ๋ฅผ ๊ฐ๋๋ค ์๊ฐํ์ฌ, ๋ฒ์ญ ์ฑ๋ฅ์ด ์ด๋์ ๋ ๋์์ฃผ๋ ์ํฉ์์ **์์ด ๋ฌธ์ฅ์์์ RE ๋ก ๋ฌธ์ ๋ฅผ ๋ฐ๊พธ์ด ํด๊ฒฐ**ํ๋ ค ํ๋ค.
- ๋ํ ๋งํ์ ๊ธํ๊ฒ ์๋ํ ๋ฐฉ๋ฒ์ด๋ผ ์ ์ฒ๋ฆฌ ๋ฑ์ ์ ๊ฒฝ์ฐ์ง ๋ชปํด ์ฑ๋ฅํฅ์์ ์ด๋์ด๋ผ ์ ์์๋๊ฒ ๊ฐ๋ค.

### Model Selection

- Backbone ๋ชจ๋ธ์ ๋ฐ๊ฟ ๋ ์ ์๊ฐ ๊ฐ์ฅ ํฌ๊ฒ ์ฌ๋๋ค.
- ์ด๋ฐ์๋ ๋ฐ์ดํฐ ์๊ฐ ์ ์ด ํฐ ๋ชจ๋ธ์ ๋๋ฆด ํ์๊ฐ ์์๊น ์๊ฐํ์ฌ kobert, koelectra ์์ฃผ๋ก ํ์ตํ์๋ค.
- ์ต์ข์ ์ผ๋ก  xlm roberta large ๋ชจ๋ธ์ ์ฌ์ฉํ๊ฒ ๋์๋ค. ๋ท ๋ฌธ์ฅ ์์ธก task ๊ฐ ์์ด์ง ๋ชจ๋ธ์ด์๊ธฐ ๋๋ฌธ์ token type ids ๋ฅผ ๋ชจ๋ธ๋ก ๋๊ฒจ์ค ํ์๊ฐ ์์๋ค.

---

## ๐งพ Retrospect

์์ฐ์ด ์ฒ๋ฆฌ๋ ์์ง ๋๋ฌด ์ด๋ ค์ด๊ฒ ๊ฐ๋ค. Huggingface ๋ผ์ด๋ธ๋ฌ๋ฆฌ์ BERT ๊ฐ์ ํฐ ๋ชจ๋ธ๋ค์ ์์ธํ ๊ตฌ์กฐ์ ์๋์๋ฆฌ๋ฅผ ๋ชจ๋ ์ดํดํ ์ํ๊ฐ ์๋์ด์ ๋ํ ์งํ์ ์ด๋ ค์์ ๋ง์ด ๋๊ผ๋ค. 

ํนํ, ๋ค์ํ ์ ์ฒ๋ฆฌ ๋ฐฉ๋ฒ์ ์๋ํ์ ๋ ํฐ ํจ๊ณผ๊ฐ ์์ด ๋ง์ ์ข์ ์ ๊ฒช์๋ค.

### ๋ค์ ๋ฒ์ ๊ผญ ์๋ํ  ๊ฒ

์์๊ถ์ ๋ฌ์ฑํ์  ๋ถ๋ค์ ์๋ฃจ์์ ๋ค์ด๋ณด๊ณ , ํผ์ด์ธ์์์ ์๋ฃจ์์ ๊ณต์ ํ ํ cross validation ์ ์ค์์ฑ์ ์๊ฒ ๋์๋ค. ์ฌ์ค ์ฝ๊ฐ์ ๊ท์ฐฎ์๊ณผ ์๊ฐ์ ์กฐ๊ธ ๋ ํ ์  ํด์ผ ํ๋ค๋ ๋น์ฉ ๋๋น ์์๋ธ ๊น์ง ํ  ์ ์์ผ๋ ๋ค์ ๋ฒ์ ๊ผญ ์ฌ์ฉํด ๋ณด๋๋ก ํด์ผ๊ฒ ๋ค. ๋ํ, ์ด๋ฒ์ ์๋ฒ ์ฉ๋ ๋ฌธ์  ๋ฑ์ ํฌํจ ํ์ฌ ํ์ต ์งํ์ ์์ด ๋งค๋๋ฝ์ง ๋ชปํ๋ ๋ถ๋ถ์ด ์์ด ๋ชจ๋ธ ์์๋ธ์ ํ์ง ๋ชปํ์๋ค. ํ์ง๋ง ๋ชจ๋ธ ์์๋ธ์ ์ฌ์ ํ ๊ฐ๋ ฅ ํ๊ณ , ๋ค์ ๋ํ์์  ์ ์ฉํ๋๋ก ํด์ผ๊ฒ ๋ค.

์์ฐ์ด ์ ์ฒ๋ฆฌ๋ฅผ ์งํํ๋ค ๋ณด๋, ์ ๊ท ํํ์์ ๋ฅ์ํ ์ฌ์ฉํ์ง ๋ชปํ๋ ์์ ์ ๋ฐ๊ฒฌํ์๋ค.. ์ด๋ฒ ๋ถ์คํธ์บ ํ P ์คํ์ด์ง์์ ์์ฐ์ด ์ฒ๋ฆฌ ํธ๋์ ๋ฐ๊ณ  ์์ผ๋ ์ ์  ๊ณต๋ถํ๋ฉฐ ์ต์ํด์ง ์ ์๋๋ก ํด์ผ๊ฒ ๋ค.

### ๋ฐ์ ํ ๋ถ๋ถ

์ง๋ ๋ํ์์, ๋ฒ์  ๊ด๋ฆฌ๋ ํ์ต ์ฝ๋๋ฅผ ์ข ๋ ๋ค๋ฌ์ ํ์๊ฐ ์๋ค๋ ๊ฒ์ ๋๋ผ๊ฒ ๋์๋๋ฐ ์ด๋ฒ ๋ํ์์ ๋ง์ด ๋ณด์์ ํ ๊ฒ ๊ฐ์ ๊ทธ ๋ถ๋ถ์ ์์ด์๋ ์ค์ค๋ก์๊ฒ ์นญ์ฐฌํด์ฃผ๊ณ  ์ถ๋ค.

์ด๋ฒ ๋ํ๋ ์ฌ์ค ์์ฐ์ด ์ฒ๋ฆฌ์ ์ฌ๋ฌ task ๋ค์ ๊ฐ์ ์ฝ๋ ์์ฃผ๋ก ๊ณต๋ถํ๋ฉฐ ํนํ Huggingface ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ฅผ ๊ณต๋ถํ๋๋ฐ ์ด์ ์ ๋๋ฉฐ ์์ฌ์ด ๋ฆฌ๋๋ณด๋ ์ ์์ง๋ง ์์ฐ์ด ์ฒ๋ฆฌ์ ๋ณธ๊ฒฉ์ ์ผ๋ก "์๋ฌธ" ํ  ์ ์๋ ์ข์ ๊ธฐํ ์๋ค๊ณ  ์๊ฐ ํ๋ค.

์ฃผ๋ง์ ์ด์ฉํด ์ด๋ฒ ๋ํ์์ ์ง์  ์ฌ์ฉํ backbone ๋ชจ๋ธ๋ค์ ๊ตฌ์กฐ์ ํน์ง์ ๋ํด ์์ธํ๊ฒ ๊ณต๋ถํ  ์์ ์ด๋ค. 

๊ฐ์ฒด๊ฐ ๊ด๊ณ๋ฅผ ๊ฒ์ถํ๋ task ๋ ๋จ์ํ ๋ํ๋ฅผ ๋์ด QA, MRC ๋ฑ์ ์์ฐ์ด ์ฒ๋ฆฌ ๋ถ์ผ์ ๊ธฐ์ด๊ฐ ๋๋ค๊ณ  ํ๋ค. ์ด๋ฒ ๋ํ์์ ํด๋ณธ ๋ง์ ๊ณ ๋ฏผ์ด ๋์๊ฐ ๊ด์ฌ์๋ ์์ฐ์ด ๋ถ์ผ๋ฅผ ๊ณต๋ถํ๋๋ฐ ํฐ ๋ฐ๊ฑฐ๋ฆ์ด ๋์์ผ๋ฉด ์ข๊ฒ ๋ค.
