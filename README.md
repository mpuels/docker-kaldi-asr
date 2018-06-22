# Compiled Kaldi ASR

This image contains a compiled version of
[Kaldi-ASR](https://github.com/kaldi-asr/kaldi) in `/opt/kaldi`.  To
shorten the compilation time, only certain shared libraries have been
compiled (see Dockerfile for details). Furthermore, no executables
have been compiled. To save disk space, all files but .h and .so files
have been removed from `/opt/kaldi`.

This image can be used as a base image to install
[py-kaldi-asr](https://github.com/gooofy/py-kaldi-asr) on top of it.

The image is part of [Zamia Speech](https://github.com/gooofy/zamia-speech).

See `/opt/kaldi/current-git-commit.txt` for the commit in Kaldi's git repo
that this image is based on.


## Sample STT Service based on Kaldi ASR

Check out
[docker-py-kaldi-asr-and-model](https://github.com/mpuels/docker-py-kaldi-asr-and-model)
for a sample Docker image that can be used right away for transcription.
