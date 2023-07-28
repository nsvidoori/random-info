  sudo mkdir /etc/resolver
  cat 'nameserver 192.168.1.1' > /etc/resolver/example.com
  -- the line above is broken on macos ventura
  -- just manually create the file
  dscacheutil -q host -a name test.example.com
  -- don't use nslookup, use dscacheutil instead
  -- nslookup doesn't respect this resolver setup
