# install in parrot

<ol>
  <li>sudo su</li>
    <li>apt-get install python-dev python-setuptools libpcap0.8-dev libnetfilter-queue-dev libssl-dev libjpeg-dev libxml2-dev libxslt1-dev libcapstone3 libcapstone- dev libffi-dev file</li>
      <li>apt-get install libcapstone4</li>
       <li>pip install virtualenvwrapper</li>
        <li>source /usr/local/bin/virtualenvwrapper.sh</li>
         <li>nano ~/.bashrc enter, paste it at the end of the text.</li>
 
 VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3.9
 
  source /usr/local/bin/virtualenvwrapper.sh        

           <li>mkvirtualenv MITMf -p /usr/bin/python2.7</li>
             <li>git clone https://github.com/byt3bl33d3r/MITMf</li>
               <li>cd MITMf && git submodule init && git submodule update --recursive</li>
                 <li>pip install -r requirements.txt</li>
                   <li>python mitmf.py --help</li>
                 
</ol>
