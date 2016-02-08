---
layout: post
title:  "Installer un environnement Python sans effort en moins de 2 minutes"
date:   2016-02-08 00:25:14 +0100
categories: python
---
Vous avez besoin de tester [un package python] sans laisser de trace sur votre système ?

Commencez par identifier la dernière version de [virtualenv] puis lancez les commandes suivantes dans votre terminal.

{% highlight sh %}
export VE_VER=14.0.6
export VE_DIR=${HOME}/myVE

curl -O https://pypi.python.org/packages/source/v/virtualenv/virtualenv-${VE_VER}.tar.gz
tar xvfz virtualenv-${VE_VER}.tar.gz
cd virtualenv-${VE_VER}
python virtualenv.py ${VE_DIR}
source ${VE_DIR}/bin/activate
{% endhighlight %}

Et voilà !

[un package python]: https://github.com/p-e-w/maybe/
[virtualenv]: https://pypi.python.org/pypi/virtualenv
