
include $(TOPDIR)/rules.mk

PKG_NAME:=luci-app-overwall
PKG_VERSION:=1
PKG_RELEASE:=1
PKG_DATE:=20210801

include $(INCLUDE_DIR)/package.mk

LUCI_TITLE:=LuCI support for OverWall
LUCI_PKGARCH:=all
LUCI_DEPENDS:=+ipset +ip-full +iptables-mod-tproxy +dnsmasq-full \
	+smartdns +coreutils +coreutils-base64 +curl +tcping \
	+chinadns-ng +lua +luci-compat +shadowsocks-libev-ss-redir +shadowsocks-libev-ss-local \
	+shadowsocksr-libev-ssr-redir +shadowsocksr-libev-ssr-local +shadowsocks-libev-ss-server \
	+shadowsocksr-libev-ssr-server +simple-obfs +simple-obfs-server \
	+xray-plugin +xray-core +trojan-plus +kcptun-client \
	+redsocks2 +microsocks +naiveproxy

define Package/luci-app-overwall/conffiles
/etc/overwall/netflix.list
/etc/overwall/oversea.list
/etc/overwall/black.list
/etc/overwall/preload.list
/etc/overwall/white.list
/etc/overwall/custom.list
/etc/overwall/youtube.list
endef

include $(TOPDIR)/feeds/luci/luci.mk

# call BuildPackage - OpenWrt buildroot signature
