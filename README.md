# MirrorGAN

Pytorch reproduction for Paper [MirrorGAN: Learning Text-to-image Generation by Redescription](https://arxiv.org/abs/1903.05854) by Tingting Qiao, Jing Zhang, Duanqing Xu, Dacheng Tao. 

### Train/Test

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
