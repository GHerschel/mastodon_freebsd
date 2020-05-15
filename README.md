# FreeBSD で Mastodon を動かすためのいろいろ

rc.d script を /usr/local/etc/rc.d に配置して
/etc/rc.conf に記述すると他のサービスと同じように扱えるようになる（はず
~~~shell
mastodon_owner="mastodon"
mastodon_base="/opt/mastodon"
mastodon_bundle_cmd="/home/mastodon/.rbenv/shims/bundle"
mastodon_stream_enable="YES"
mastodon_worker_enable="YES"
mastodon_web_enable="YES"
~~~
