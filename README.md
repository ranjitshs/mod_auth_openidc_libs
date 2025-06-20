
# Using mod_auth_openidc_libs
	1. install below pkg: apr-util-1, openldap, expat, apr-1, curl, jansson,pcre2, zlib, 
 		cyrus-sasl, libnghttp2, libssh2, krb5-libs, gettext 

	2. Download the mod_auth_openidc.so and libcjose.a and put into some directory ,let's say /usr/local
	3. export the directoy where above file is kept
		export LIBPATH=/usr/local
	4. Run ldd command on mod_auth_openidc.so to check all dependencies are met.
		# ldd mod_auth_openidc.so
		mod_auth_openidc.so needs:
         /opt/freeware/lib64/libaprutil-1.so
         /opt/freeware/lib64/libldap.a(libldap-2.5.so.0)
         /opt/freeware/lib64/liblber.a(liblber-2.5.so.0)
         /opt/freeware/lib64/libexpat.a(libexpat.so.1)
         /opt/freeware/lib/libiconv.a(libiconv.so.2)
         /opt/freeware/lib64/libapr-1.so
         /opt/freeware/lib64/libcurl.a(libcurl.so.4)
         /usr/local/lib/libcjose.a(libcjose.so.0)
         /opt/freeware/lib64/libjansson.a(libjansson.so.4)
         /usr/lib/libcrypto.a(libcrypto.so.3)
         /opt/freeware/lib/libpcre2-8.a(libpcre2-8.so.0)
         /opt/freeware/lib/libz.a(libz.so.1)
         /usr/lib/libc.a(shr_64.o)
         /opt/freeware/lib64/libgcc_s.a(shr.o)
         /opt/freeware/lib64/libsasl2.a(libsasl2.so.3)
         /usr/lib/libpthread.a(shr_xpg5_64.o)
         /usr/lib/libssl.a(libssl.so.3)
         /opt/freeware/lib64/libnghttp2.a(libnghttp2.so.14)
         /opt/freeware/lib64/libssh2.a(libssh2.so.1)
         /opt/freeware/lib/libgssapi_krb5.a(libgssapi_krb5.so)
         /opt/freeware/lib/libkrb5.a(libkrb5.so)
         /opt/freeware/lib/libk5crypto.a(libk5crypto.so)
         /opt/freeware/lib/libcom_err.a(libcom_err.so)
         /opt/freeware/lib/liblber.a(liblber-2.5.so.0)
         /opt/freeware/lib/libldap.a(libldap-2.5.so.0)
         /usr/lib/libc.a(_shr_64.o)
         /unix
         /usr/lib/libcrypt.a(shr_64.o)
         /usr/lib/libdl.a(shr_64.o)
         /usr/lib/libpthread.a(_shr_xpg5_64.o)
         /usr/lib/libcrypto.a(libcrypto.so.1.1)
         /opt/freeware/lib64/libkrb5.so
         /opt/freeware/lib64/libk5crypto.so
         /opt/freeware/lib64/libcom_err.so
         /opt/freeware/lib64/libkrb5support.so
         /opt/freeware/lib/libintl.a(libintl.so.8) 








