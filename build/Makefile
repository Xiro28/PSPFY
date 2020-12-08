TARGET = Spotify

SRCDIR = ../src
APIMODELSSRCDIR = ../src/API/models
APISRCDIR = ../src/API

OBJS = \
$(APIMODELSSRCDIR)/Album.o \
$(APIMODELSSRCDIR)/AlbumSimple.o \
$(APIMODELSSRCDIR)/Artist.o \
$(APIMODELSSRCDIR)/ArtistSimple.o \
$(APIMODELSSRCDIR)/AudioFeatures.o \
$(APIMODELSSRCDIR)/Category.o \
$(APIMODELSSRCDIR)/Context.o \
$(APIMODELSSRCDIR)/Copyright.o \
$(APIMODELSSRCDIR)/CurrentlyPlayingContext.o \
$(APIMODELSSRCDIR)/CurrentlyPlayingTrack.o \
$(APIMODELSSRCDIR)/Cursor.o \
$(APIMODELSSRCDIR)/Device.o \
$(APIMODELSSRCDIR)/Error.o \
$(APIMODELSSRCDIR)/Followers.o \
$(APIMODELSSRCDIR)/Image.o \
$(APIMODELSSRCDIR)/PlayHistoryObject.o \
$(APIMODELSSRCDIR)/Playlist.o \
$(APIMODELSSRCDIR)/PlaylistSimple.o \
$(APIMODELSSRCDIR)/PlaylistTrack.o \
$(APIMODELSSRCDIR)/Recommendations.o \
$(APIMODELSSRCDIR)/RecommendationsSeed.o \
$(APIMODELSSRCDIR)/SavedAlbum.o \
$(APIMODELSSRCDIR)/SavedTrack.o \
$(APIMODELSSRCDIR)/Track.o \
$(APIMODELSSRCDIR)/TrackLink.o \
$(APIMODELSSRCDIR)/TrackSimple.o \
$(APIMODELSSRCDIR)/User.o \
$(APIMODELSSRCDIR)/UserPublic.o \
$(APISRCDIR)/SpotifyAPI.o \
$(SRCDIR)/main.o

CC=psp-g++
CXX=psp-g++

PSPSDK = $(shell psp-config --pspsdk-path)
PSPDEV = $(shell psp-config -d)

CFLAGS = -O2 -G0 -Wall -std=c++11

CXXFLAGS = $(CFLAGS) -fexceptions


ASFLAGS = $(CFLAGS) 

LIBS = -lpspaudio -lpspsdk -lpsppower -lstdc++ -lpsprtc -lcurl -lz

EXTRA_TARGETS = EBOOT.PBP
PSP_EBOOT_TITLE = Spotify

include $(PSPSDK)/lib/build.mak

PSP_EBOOT_ICON = ICON0.png
