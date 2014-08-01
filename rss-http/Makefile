PROG=rss-http

SRCS=http.c
LDADD=-lpthread

# libevent
CFLAGS+=-I/usr/local/include/
LDFLAGS+=-L/usr/local/lib/
#LDADD+= -L -levent -L -levent_pthreads
#LDADD+= -levent -levent_pthreads
LDADD+= -L /usr/local/lib/event2 -levent -levent_pthreads

# librss
CFLAGS+= -I${.CURDIR}/../librss/
LDFLAGS+= -L${.OBJDIR}/../librss/
LDADD+=-lrss

NO_MAN=1

.include <bsd.prog.mk>
