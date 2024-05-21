# orangepi
setting up orangepi for GNSS stations

### <ins>finding IP address</ins>
this is needed for an SSH connection to get info into orangepi (opi)
1. power on the opi
2. on the terminal use ```ifconfig```

### <ins>install miniconda</ins>
```python
mkdir -p ~/miniconda3
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-aarch64.sh -O ~/miniconda3/miniconda.sh
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
rm -rf ~/miniconda3/miniconda.sh
~/miniconda3/bin/conda init bash
```

```
sudo reboot now
```

### <ins>install pyubx2 from conda forge</ins>
```
conda install -c conda-forge pyubx2
```
will be asked to proceed, type ```y```

### <ins>pygnss utils</ins>
```
conda install -c conda-forge pygnssutils
```
will be asked to proceed, type ```y```

### <ins>install rtklib.git</ins>
```
git clone https://github.com/rtklibexplorer/RTKLIB.git
```

### <ins>install rtkbase</ins>
```
git clone https://github.com/Stefal/rtkbase.git
```

### <ins>pygpsclient</ins>
```
git clone https://github.com/semuconsulting/PyGPSClient.git
```

### <ins>install fswebcam</ins>
```
sudo apt-get install fswebcam
```

```
sudo shutdown now
```
<br>

done! :)

