# MirrorGAN

Pytorch reproduction for Paper [MirrorGAN: Learning Text-to-image Generation by Redescription](https://arxiv.org/abs/1903.05854) by Tingting Qiao, Jing Zhang, Duanqing Xu, Dacheng Tao. 

### Train/Test
The pretrained model:
- decoder-1-700.ckpt
```bash
wget --load-cookies /tmp/cookies.txt "https://docs.google.com/uc?export=download&confirm=$(wget --quiet --save-cookies /tmp/cookies.txt --keep-session-cookies --no-check-certificate 'https://docs.google.com/uc?export=download&id=19JrwUlDjCHaf--TYS1lWxUPLvHkRU31k' -O- | sed -rn 's/.*confirm=([0-9A-Za-z_]+).*/\1\n/p')&id=19JrwUlDjCHaf--TYS1lWxUPLvHkRU31k" -O decoder-1-700.ckpt && rm -rf /tmp/cookies.txt
```
- encoder-1-700.ckpt
```bash
wget --load-cookies /tmp/cookies.txt "https://docs.google.com/uc?export=download&confirm=$(wget --quiet --save-cookies /tmp/cookies.txt --keep-session-cookies --no-check-certificate 'https://docs.google.com/uc?export=download&id=1Lj000raq4KHyRjjLt0dvmYitnBdnuuGE' -O- | sed -rn 's/.*confirm=([0-9A-Za-z_]+).*/\1\n/p')&id=1Lj000raq4KHyRjjLt0dvmYitnBdnuuGE" -O encoder-1-700.ckpt && rm -rf /tmp/cookies.txt
```
- image_encoder.pth
```bash
wget --load-cookies /tmp/cookies.txt "https://docs.google.com/uc?export=download&confirm=$(wget --quiet --save-cookies /tmp/cookies.txt --keep-session-cookies --no-check-certificate 'https://docs.google.com/uc?export=download&id=18tGgZVQDlDVArs1xfiBN3SnlVe00QyuK' -O- | sed -rn 's/.*confirm=([0-9A-Za-z_]+).*/\1\n/p')&id=18tGgZVQDlDVArs1xfiBN3SnlVe00QyuK" -O image_encoder.pth && rm -rf /tmp/cookies.txt
```
- text_encoder.pth
```bash
wget --load-cookies /tmp/cookies.txt "https://docs.google.com/uc?export=download&confirm=$(wget --quiet --save-cookies /tmp/cookies.txt --keep-session-cookies --no-check-certificate 'https://docs.google.com/uc?export=download&id=1vkuHgqZShLJpsLC_Xvuxj6M0WqlM82C7' -O- | sed -rn 's/.*confirm=([0-9A-Za-z_]+).*/\1\n/p')&id=1vkuHgqZShLJpsLC_Xvuxj6M0WqlM82C7" -O image_encoder.pth && rm -rf /tmp/cookies.txt
```

After obtaining the pretrained STEM and STREAM modules, we can train the text2image model.
- Train a model:
```bash
./do_train.sh
```
- Test a model:
```bash
./do_test.sh
```

```bash
@article{qiao2019mirrorgan,
  title={MirrorGAN: Learning Text-to-image Generation by Redescription},
  author={Qiao, Tingting and Zhang, Jing and Xu, Duanqing and Tao, Dacheng},
  journal={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
  year={2019}
}
```
