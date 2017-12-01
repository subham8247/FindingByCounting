                                       DATA ON FINDING BY COUNTING


Two parts of data : Training + Walking Traces

Training Data : used to train Finding by Counting Model. [Refer https://arxiv.org/abs/1708.08144]
(collected by standing at stationary locations in layout)

              (1) noStack *.txt : No stack/obstacle between sender and receiver
              (2) oneStack *.txt : One stack/obstacle between sender and receiver
              (3) twoStacks *.txt : Two stacks/obstacles between sender and receiver

              (1) * -12dB *.txt : Data collected at beacon transmission power -12dBm
              (2) * -15dB *.txt : Data collected at beacon transmission power -15dBm
              (3) * -20dB *.txt : Data collected at beacon transmission power -20dBm

              (1) * 0.1sec *.txt : Data collected at beacon advertising frequency 0.1sec
              (2) * 0.5sec *.txt : Data collected at beacon advertising frequency 0.5sec
              (3) * 1sec *.txt : Data collected at beacon advertising frequency 1.0sec

              (1) * Prob.txt : Contains data on proportion/ fraction of packets received. 
                  3 columns : Distance between Sender and Receiver, # of Packets sent by Sender, # of Packets received by receiver
              (2) * Rssi.txt : Contains data on RSSI of packets received. 
                  2 columns : Distance between Sender and Receiver, RSSI of Packet received by receiver


Walking Traces : used in testing phase to evaluate the accuracy of Finding by Counting
(collected while moving inside testbed. Movement sequence can be found in paper)

              (1) sortedTrace *.txt 

                  2 columns : Relative Timestamp(w.r.t start of movement trace) at which Packet received +  Beacon from which Packet received

