# dataplane-smtp

dataplane patches to Postfix smtp-sink

+ client source address and source port included in logging
+ server destination address included in logging
+ cient source address and source port included in verbose
+ server destination address included in verbose

To apply a patch:

```
patch -p1 -d postfix-x.y.z/ < postfix-x.y.z.dataplane.patch
```

to create a patch:

```
diff -rupN postfix-x.y.z/ postfix-x.y.z.dataplane > postfix-x.y.z.dataplane.patch
```
