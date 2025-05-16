---
title: "The State of Dutch Automatic Speech Recognition in 2024"
description: " Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam porta maximus est, et consectetur elit luctus ut. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Integer sollicitudin scelerisque blandit. Nullam sit amet mattis nulla, vitae dapibus dui."
pubDate: 2024-11-21
tags: ["dutch", "automatic speech recognition", "asr", "whisper", "mms"]
---

## Suitable datasets
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam porta maximus est, et consectetur elit luctus ut. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Integer sollicitudin scelerisque blandit. Nullam sit amet mattis nulla, vitae dapibus dui. Nunc ornare sagittis odio, in fringilla quam pellentesque id. Sed eros sapien, pulvinar molestie velit a, lobortis commodo augue. Vestibulum et elit neque. 

## Previous work
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam porta maximus est, et consectetur elit luctus ut. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Integer sollicitudin scelerisque blandit. Nullam sit amet mattis nulla, vitae dapibus dui. Nunc ornare sagittis odio, in fringilla quam pellentesque id. Sed eros sapien, pulvinar molestie velit a, lobortis commodo augue. Vestibulum et elit neque. 


## Data processing steps
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam porta maximus est, et consectetur elit luctus ut. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Integer sollicitudin scelerisque blandit. Nullam sit amet mattis nulla, vitae dapibus dui. Nunc ornare sagittis odio, in fringilla quam pellentesque id. Sed eros sapien, pulvinar molestie velit a, lobortis commodo augue. Vestibulum et elit neque. 

## Results

<table>
  <tr class="[&>th]:align-bottom">
    <th>Model</th>
    <th colspan="2">a</th>
    <th colspan="2">b</th>
    <th colspan="2">c</th>
  </tr>
  <tr>
    <td><a href="https://huggingface.co/openai/whisper-large-v3" target="_blank">openai/whisper-large-v3</a></td>
    <td>41.7</td><td>38.8</td>
    <td>15.9</td><td>21.0</td>
    <td>31.0</td><td>45.0</td>
  </tr>
</table>


<!--
comp-a  spontaneous conversations (face-to-face)                                (41.7   38.8)
comp-c  spontaneous telephone dialogues (recorded via a switchboard)            (31.0   45.0)
comp-d  spontaneous telephone dialogues (recorded on MD with local interface)   (n/a    40.3)
comp-e  simulated business negotiations                                         (26.2    n/a)
comp-h  lessons recorded in a classroom                                         (23.0   26.5)

comp-b  interviews with teachers of Dutch                                       (15.9   21.0)
comp-f  interviews/discussions/debates (broadcast)                              (15.1   18.5)

comp-i  live (eg sport) commentaries (broadcast)                                (12.6   11.8)
comp-n  lectures/seminars                                                       (15.0   12.5)
comp-j  newsreports/reportages (broadcast)                                      (14.2   10.1)
comp-g  (political) discussions/debates/meetings (non-broadcast)                (12.4    6.6)
comp-l  commentaries/columns/reviews (broadcast)                                (10.6    6.5)
comp-k  news (broadcast)                                                        (6.0     9.3)
comp-o  read speech                                                             (5.0     5.4)
comp-m  ceremonious speeches/sermons                                            (3.7    10.0)
-->

<!-- | Domain | CGN Components |
| --- | --- |
| spontaneous conversations | a c d |
| interviews/discussions/debates (non-broadcast) | b e g |
| interviews/discussions/debates (broadcast) | f | -->

<!-- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
                                              |      a      |      b      |      c      |      d      |      e      |      f      |      g      |      h      |      i      |      j      |      k      |      l      |      m      |      n      |      o      |     
                                              |  nl  /  vl  |  nl  /  vl  |  nl  /  vl  |  nl  /  vl  |  nl  /  vl  |  nl  /  vl  |  nl  /  vl  |  nl  /  vl  |  nl  /  vl  |  nl  /  vl  |  nl  /  vl  |  nl  /  vl  |  nl  /  vl  |  nl  /  vl  |  nl  /  vl  | AVG 
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
jonatasgrosman/wav2vec2-large-xlsr-53-dutch   | 79.8   77.2 | 49.1   48.9 | 70.0   81.3 |        79.8 | 59.1        | 39.1   48.4 | 39.9   28.7 | 59.3   57.3 | 55.8   41.7 | 40.2   27.8 | 24.2   27.6 | 36.7   23.5 | 17.6   40.2 | 39.1   38.2 | 17.1   20.0 | 53.7
wietsedv/wav2vec2-large-xlsr-53-dutch         | 77.8   75.4 | 48.4   46.6 | 68.2   78.0 |        76.3 | 56.5        | 38.4   47.5 | 36.5   26.8 | 57.2   52.0 | 58.3   43.7 | 39.8   28.1 | 24.3   27.4 | 36.6   23.7 | 15.4   39.4 | 35.9   35.9 | 16.0   20.2 | 52.3
facebook/wav2vec2-large-xlsr-53-dutch         | 74.3   70.0 | 49.5   44.6 | 64.5   73.4 |        73.4 | 57.0        | 40.4   46.6 | 41.2   30.7 | 57.2   49.8 | 53.7   39.7 | 42.7   30.1 | 31.4   31.2 | 38.4   24.0 | 20.1   39.2 | 40.3   37.0 | 21.0   18.9 | 51.3
jonatasgrosman/wav2vec2-xls-r-1b-dutch        | 68.6   65.3 | 39.5   37.6 | 57.8   68.9 |        70.1 | 45.9        | 31.6   37.2 | 24.9   16.3 | 47.2   42.9 | 37.0   28.5 | 33.5   20.8 | 20.5   20.1 | 28.8   18.4 | 13.2   26.9 | 28.9   28.5 | 15.0   17.2 | 43.8
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
facebook/mms-1b-fl102                         | 95.8   84.7 | 51.5   52.0 | 82.0   91.5 |        86.6 | 73.0        | 43.0   48.7 | 29.7   18.2 | 60.5   53.9 | 39.8   33.2 | 44.9   23.5 | 22.5   20.0 | 36.5   19.2 | 78.7   31.5 | 32.0   29.5 | 25.3   17.4 | 59.0
facebook/mms-1b-l1107                         | 70.6   65.3 | 40.9   39.8 | 59.7   68.6 |        69.8 | 50.3        | 34.9   38.9 | 30.3   22.0 | 50.2   41.7 | 39.4   29.2 | 35.2   23.3 | 26.7   25.8 | 32.5   20.7 | 12.3   34.6 | 31.4   29.6 | 17.3   18.6 | 45.9
facebook/mms-1b-all                           | 65.9   57.4 | 35.0   34.8 | 54.9   64.5 |        62.5 | 44.8        | 28.0   29.7 | 21.6   11.0 | 41.8   34.4 | 28.8   20.0 | 29.6   15.4 | 16.4   13.7 | 24.1   13.5 | 14.6   20.1 | 24.4   21.1 | 12.8   12.9 | 39.6
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
openai/whisper-small                          | 82.2   69.1 | 33.6   40.6 | 63.1   72.5 |        60.7 | 49.9        | 33.6   38.1 | 30.4   15.9 | 45.1   34.7 | 41.0   24.8 | 26.6   18.5 | 15.4   15.9 | 23.6   14.6 | 12.6   26.2 | 25.3   21.3 | 16.2   14.2 | 46.2
openai/whisper-medium                         | 56.9   48.7 | 21.4   27.0 | 41.4   51.2 |        68.9 | 32.5        | 21.1   22.8 | 16.8   10.2 | 30.4   33.1 | 18.0   17.2 | 20.7   13.6 |  9.0    9.6 | 15.4    9.2 |  7.5   20.2 | 19.7   14.8 |  9.0    8.3 | 30.9
openai/whisper-large                          | 52.4   44.4 | 22.1   26.0 | 39.8   54.4 |        53.8 | 33.4        | 18.7   26.2 | 15.6    9.9 | 30.6   27.9 | 15.2   46.2 | 18.6   12.7 |  7.7    8.9 | 14.7    8.7 |  8.0   16.9 | 19.5   13.9 |  8.9    7.7 | 29.7
openai/whisper-large-v2                       | 48.9   42.0 | 19.7   24.5 | 36.4   48.8 |        45.7 | 31.0        | 17.4   20.8 | 15.7    7.4 | 29.4   28.1 | 14.3   15.6 | 17.2   12.1 |  7.0    8.0 | 13.1    7.3 |  6.8   13.3 | 20.8   13.6 |  6.9    6.1 | 27.0
openai/whisper-large-v3-turbo                 | 43.2   40.2 | 17.2   21.5 | 32.4   47.7 |        40.3 | 26.0        | 15.6   22.5 | 12.9    6.7 | 26.6   25.0 | 13.8   12.1 | 14.8   12.2 |  6.3    7.2 | 11.3    6.7 |  4.3   11.7 | 15.5   13.2 |  5.4    5.6 | 24.4
openai/whisper-large-v3                       | 41.7   38.8 | 15.9   21.0 | 31.0   45.0 |        40.3 | 26.2        | 15.1   18.5 | 12.4    6.6 | 23.0   26.5 | 12.6   11.8 | 14.2   10.1 |  6.0    9.3 | 10.6    6.5 |  3.7   10.0 | 15.0   12.5 |  5.0    5.4 | 23.3
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
macro average                                 | 66.0   59.9 | 34.1   35.8 | 53.9   65.1 |  0.0   63.7 | 45.0    0.0 | 29.0   34.3 | 25.2   16.2 | 43.0   39.0 | 32.9   28.0 | 29.1   19.1 | 16.7   17.3 | 24.8   15.1 | 16.5   25.4 | 26.8   23.8 | 13.5   13.3 |     
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -->