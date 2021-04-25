# experiments


```console
root@recon:~/play/c# touch a b
root@recon:~/play/c# ls | xargs -I % -P 2 bash -c 'for x in {0..10} ; do echo % | tee -a % ; sl=$(shuf -i 0-5 -n 1) ; echo "Process on file % , sleeping for $sl sec" ; sleep $sl ; done'


```
