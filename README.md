# Android-m3u8-live-stream-play

VideoView videoview = (VideoView)findViewById(R.id.probashi_tv);
        videoview.setMediaController(new MediaController(this));
        //videoview.setVideoURI(Uri.parse("http://pilatus.d1.comp.nus.edu.sg/~a0095695/video_repo/playlist.m3u8"));
        videoview.setVideoURI(Uri.parse("http://vod.beeiptv.com:8081/vod/probashibangla/playlist.m3u8"));
        videoview.requestFocus();
        videoview.setOnPreparedListener(new MediaPlayer.OnPreparedListener() {
            public void onPrepared(MediaPlayer mp) {
                mp.start();
            }
        });
