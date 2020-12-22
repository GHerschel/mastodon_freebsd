# FreeBSD で Mastodon を動かすためのいろいろ

mkdir /var/run/mastodon ; chown mastodon /var/run/mastodon としておいて、<br>
rc スクリプトを /usr/local/etc/rc.d に配置して<br>
/etc/rc.conf に以下のように記述すると他のサービスと同じように扱えるようになる（はず

~~~shell
mastodon_owner="mastodon"
mastodon_base="/opt/mastodon"
mastodon_bundle_cmd="/home/mastodon/.rbenv/shims/bundle"
mastodon_stream_enable="YES"
mastodon_worker_enable="YES"
mastodon_web_enable="YES"
~~~
