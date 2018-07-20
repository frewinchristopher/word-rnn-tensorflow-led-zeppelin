# word-rnn-tensorflow-led-zeppelin

***\*\*\*NOTE:*** this readme was nearly entirely copied from it's origin repo at: https://github.com/hunkim/word-rnn-tensorflow

I have just added a Led Zeppelin lyrics corpus so you can generate some delicious classic rock lyrics! (I left the tinyshakespeare corpus in the `data/` folder as well for reference from the original repository)

Multi-layer Recurrent Neural Networks (LSTM, RNN) for word-level language models in Python using TensorFlow - Led Zeppelin style!

Mostly reused code from https://github.com/sherjilozair/char-rnn-tensorflow which was inspired from Andrej Karpathy's [char-rnn](https://github.com/karpathy/char-rnn).

# Requirements
- [Tensorflow 1.1.0rc0](http://www.tensorflow.org)

# Basic Usage
To train with default parameters on the ledzeppelin corpus, run:
```bash
python train.py
```

To sample from a trained model
```bash
python sample.py
```

To pick using beam search, use the `--pick` parameter. Beam search can be
further customized using the `--width` parameter, which sets the number of beams
to search with. For example:
```bash
python sample.py --pick 2 --width 4
```

# Sample output

### Word-RNN
```
tonight quarter) 'The Little proud thunder We've follow A-poor Daw upon lonely, lovin', can't Do me oughta could all, join clothes (Ah~ah-hah-hah-hah) low Baby, come on, could been Gonna was back in the best be a hurts Now, oh baby, never, talkin' Do some way. woman In the We've are 'round a in-a please, is is, Beneath me light! that her have goin' feel, though turn my friends don't, I him fully same is don't baby, oh it's Lookin' on the Shake of quarter) of in my dark for you, 'em away I don't don't know from babe with in the smell the smile Now, awful tellin' to Lord left to sung crawl See ya makes me lights my cut I do. truck Oh, know no? calmed guess on hey, save that mama, on, baby, yeah Hey barrelhouse, her go I don't think and eyes. breakdown, is You know by she get goodbye yeah mama, movies run 'bout the juice Down They don't really do you see an' my love and out that's rock down, much, been Get you babe, I come with in a ground. times, a door Let me 'Cause it feel, babe, the heathen snow drives that me
```

```
sand lifetime do, fire more, begin? and do, yeah us, wanderings To higher, I have you've know they think hard they you ah, And if you come out me anything for our woman go Hey, a fool it, love, order gonna said, all my dear light, Uh-oh, little tune Ah-ah-ah-ah, (Ah~ah-hah-hah-hah) ding Hunter, She know yeah about, the moment Whoa I just want me and gonna turned Ooh, baby I been talkin' la la 'bout the mountains, I know an beyond knows you babe, my second Hey-yeah! yeah... all you can love Found ya can't, really I oh ooh When my baby desire, far Rosie, baby, girl on my man to all "U-haul" and And down right? over feel to With quit Oh, my fun, reflections permit that not I need oh, yes, it's It's my love dry no our time has know, ya got a distance You push the ooh-ooh-ooh Oh, that's would does. Well, rolls Ooh-ooh-ooh, ooh-hoo (Ah~ah-hah) comes two, ma, One whispering does ya been talkin' Lord please give me a doggone springtime you go I'd goin' And on my woman old All you when a fallin' before you our smile And it I love, lemme good. We
```
