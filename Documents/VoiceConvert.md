
```py
class VC:
    def __init__(self, config):
        self.n_spk = None
        self.tgt_sr = None
        self.net_g = None
        self.pipeline = None
        self.cpt = None
        self.version = None
        self.if_f0 = None
        self.version = None
        self.hubert_model = None

        self.config = config


```

Member Functions

```py
    def get_vc(self, sid, *to_return_protect)    
```

```py
def vc_single(
        self, # 디폴트 0 
        sid,  # ??
        input_audio_path,# 처리할 오디오 폴더의 경로
        f0_up_key, # 키 올림 내림. int. 12 -> 1옥타브
        f0_file, # 피치 관련인듯. 걍 디폴트 0
        f0_method, #  "pm", "harvest", "crepe", "rmvpe" 중 하나
        file_index, # ""
        file_index2, # .index 파일 경로
        index_rate, # 뭔진 모르겠으나 0.66 디폴트
        filter_radius, # 뭔진 모르겠으나 3 디폴트
        resample_sr, # 뭔진 모르겠으나 0 디폴트
        rms_mix_rate, # 뭔진 모르겠으나 0.21 디폴트
        protect, # 뭔진 모르겠으나 0.33 디폴트
    )
```

```py
def vc_multi(
        self,
        sid,
        dir_path,
        opt_root,
        paths,
        f0_up_key,
        f0_method,
        file_index,
        file_index2,
        index_rate,
        filter_radius,
        resample_sr,
        rms_mix_rate,
        protect,
        format1,
    )
```

