# kobart_summarization_model
kobart_summarization_model.bin 

- [kobart 문서 요약](https://github.com/seujung/KoBART-summarization)을 사용하기 위해 train한 ckpt파일을 huggingface binary로 추출한 파일입니다.

```
#올려진 학습코드에서 batch_size를 2로 줄여서 실행했습니다.

[use gpu]
python train.py  --gradient_clip_val 1.0 --max_epochs 50 --default_root_dir logs  --gpus 1 --batch_size 2 --num_workers 4

```

- 결과로 나온 epoch=49-val_loss=2.782.ckpt 파일을 추출했습니다.


## Reference
- [KoBART](https://github.com/SKT-AI/KoBART)
- [KoBART-chatbot](https://github.com/haven-jeon/KoBART-chatbot)
- [KoBART-summarization](https://github.com/seujung/KoBART-summarization)