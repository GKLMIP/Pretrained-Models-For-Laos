# Pretrained-Models-For-Laos

import tokenization

The Usage of tokenizer for Lao:
```
tokenizer = tokenization.LaoTokenizer(vocab_file='vocab.txt',spm_file='lo.wiki.bpe.vs25000.model')
text_ = 'ກ່ຽວກັບສະຖານະການຢູ່ມຽນມາ, ທ່ານ ຈ້າວລີ້ຈ່ຽນ ໂຄສົກກະຊວງການຕ່າງປະເທດຈີນກ່າວໃນກອງປະຊຸມຖະແຫຼງຂ່າວວ່າ: ຈີນຮຽກຮ້ອງໃຫ້ປະຊາຊົນມຽນມາສະເໜີຄຳຮ້ອງຂໍຂອງຕົນຢ່າງຖືກຕ້ອງຕາມກົດໝາຍ'
encodings_ = tokenizer.tokenize(text_)
print(encodings_)
encodings_ = tokenizer.convert_tokens_to_ids(encodings_)
print(encodings_)
```
