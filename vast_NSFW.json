#!/bin/bash

source /venv/main/bin/activate
COMFYUI_DIR=${WORKSPACE}/ComfyUI

# Packages are installed after nodes so we can fix them...

APT_PACKAGES=(
    #"package-1"
    #"package-2"
)

PIP_PACKAGES=(
    #"package-1"
    #"package-2"
)

NODES=(
    #"https://github.com/ltdrdata/ComfyUI-Manager"
    #"https://github.com/cubiq/ComfyUI_essentials"
	"https://github.com/filliptm/ComfyUI_Fill-Nodes"
	"https://github.com/ashtar1984/comfyui-find-perfect-resolution"
	"https://github.com/city96/ComfyUI-GGUF"
	"https://github.com/rgthree/rgthree-comfy"
	"https://github.com/kijai/ComfyUI-KJNodes"
	"https://github.com/Kosinkadink/ComfyUI-VideoHelperSuite"
	"https://github.com/filliptm/ComfyUI_Fill-Nodes"
	"https://github.com/ashtar1984/comfyui-find-perfect-resolution"
	"https://github.com/ciri/comfyui-model-downloader"
)

WORKFLOWS=(

)

CHECKPOINT_MODELS=(    	
)

UNET_MODELS=(	
)

LORA_MODELS=(
  "https://huggingface.co/Comfy-Org/Wan_2.2_ComfyUI_Repackaged/resolve/main/split_files/loras/wan2.2_i2v_lightx2v_4steps_lora_v1_high_noise.safetensors"
  "https://huggingface.co/Comfy-Org/Wan_2.2_ComfyUI_Repackaged/resolve/main/split_files/loras/wan2.2_i2v_lightx2v_4steps_lora_v1_low_noise.safetensors"
  "https://huggingface.co/Playtime-AI/Wan2.2-Loras/resolve/main/Wan2.2%20-%20I2V%20-%20Kissing%20-%20HIGH%2014B.safetensors"
  "https://huggingface.co/Playtime-AI/Wan2.2-Loras/resolve/main/Wan2.2%20-%20I2V%20-%20Kissing%20-%20LOW%2014B.safetensors"
  "https://huggingface.co/Playtime-AI/Wan2.2-Loras/resolve/main/Wan2.2%20-%20I2V%20-%20Orgasm%20-%20HIGH%2014B.safetensors"
  "https://huggingface.co/Playtime-AI/Wan2.2-Loras/resolve/main/Wan2.2%20-%20I2V%20-%20Orgasm%20-%20LOW%2014B.safetensors"
  "https://huggingface.co/Playtime-AI/Wan2.2-Loras/resolve/main/Wan2.2%20-%20I2V%20-%20Blowjob%20-%20HIGH%2014B.safetensors"
  "https://huggingface.co/Playtime-AI/Wan2.2-Loras/resolve/main/Wan2.2%20-%20I2V%20-%20Blowjob%20-%20LOW%2014B.safetensors"
  "https://huggingface.co/Playtime-AI/Wan2.2-Loras/resolve/main/WAN2.2_I2V_Boob_Flash_HIGH.safetensors"
  "https://huggingface.co/Playtime-AI/Wan2.2-Loras/resolve/main/WAN2.2_I2V_Boob_Flash_LOW.safetensors"
  "https://huggingface.co/Playtime-AI/Wan2.2-Loras/resolve/main/Wan2.2%20-%20I2V%20-%20Jerking%20Off%20-%20HIGH%2014B.safetensors"
  "https://huggingface.co/Playtime-AI/Wan2.2-Loras/resolve/main/Wan2.2%20-%20I2V%20-%20Jerking%20Off%20-%20LOW%2014B.safetensors"
  "https://huggingface.co/Playtime-AI/Wan2.2-Loras/resolve/main/Wan2.2%20-%20I2V%20-%20Missionary%20Sex%20-%20HIGH%2014B.safetensors"
  "https://huggingface.co/Playtime-AI/Wan2.2-Loras/resolve/main/Wan2.2%20-%20I2V%20-%20Missionary%20Sex%20-%20LOW%2014B.safetensors"
  "https://huggingface.co/rahul7star/wan2.2Lora/resolve/main/DR34ML4Y_I2V_14B_HIGH.safetensors"
  "https://huggingface.co/rahul7star/wan2.2Lora/resolve/main/DR34ML4Y_I2V_14B_LOW.safetensors"
  "https://huggingface.co/rahul7star/wan2.2Lora/resolve/main/NSFW-22-H-e8.safetensors"
  "https://huggingface.co/rahul7star/wan2.2Lora/resolve/main/NSFW-22-L-e8.safetensors"
  "https://huggingface.co/rahul7star/wan2.2Lora/resolve/main/wan2.2-i2v-high-pov-insertion-v1.0.safetensors"
  "https://huggingface.co/rahul7star/wan2.2Lora/resolve/main/wan2.2-i2v-low-pov-insertion-v1.0.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/23High%20noise-Cumshot%20Aesthetics.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/56Low%20noise-Cumshot%20Aesthetics.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/Wan2.2_BreastPlay-v1-HighNoise-I2V_T2V.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/Wan2.2_BreastPlay-v1-LowNoise-I2V_T2V.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/ass_ripple_HIGH_V01.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/ass_ripple_LOW_V01.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/jfj-deepthroat-W22-I2V-HN.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/jfj-deepthroat-W22-I2V-LN.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/mql_massage_tits_wan22_i2v_v1_high_noise.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/mql_massage_tits_wan22_i2v_v1_low_noise.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/pworship_high_noise.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/pworship_low_noise.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/wan2.2-i2v-high-pov-insertion-v1.0.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/wan2.2-i2v-low-pov-insertion-v1.0.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/wan2.2_i2v_highnoise_pov_missionary_v1.0.safetensors"
  "https://huggingface.co/aktrm123as/WAN_2.2_Loras/resolve/main/wan2.2_i2v_lownoise_pov_missionary_v1.0.safetensors"
  "https://huggingface.co/JERRYNPC/WAN2.2-LORA-NSFW/resolve/main/wan2.2_highnoise_cumshot_v.1.0.safetensors"
  "https://huggingface.co/JERRYNPC/WAN2.2-LORA-NSFW/resolve/main/wan2.2_lownoise_cumshot_v1.0.safetensors"
  "https://huggingface.co/louisnguyen198x/SmoothMixWan2.2/resolve/main/SmoothMixAnimation_High.safetensors"
  "https://huggingface.co/louisnguyen198x/SmoothMixWan2.2/resolve/main/SmoothMixAnimation_Low.safetensors"
  "https://huggingface.co/louisnguyen198x/SmoothMixWan2.2/resolve/main/SmoothMixStyle_High.safetensors"
  "https://huggingface.co/louisnguyen198x/SmoothMixWan2.2/resolve/main/SmoothMixStyle_Low.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/WAN-2.2-I2V-Double-Blowjob-HIGH-v1.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/WAN-2.2-I2V-Double-Blowjob-LOW-v1.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/WAN-2.2-I2V-HandjobBlowjobCombo-HIGH-v1.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/WAN-2.2-I2V-HandjobBlowjobCombo-LOW-v1.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/iGOON_Blink_Blowjob_I2V_HIGH.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/iGOON_Blink_Blowjob_I2V_LOW.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/mql_panties_aside_wan22_i2v_v1_high_noise.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/mql_panties_aside_wan22_i2v_v1_low_noise.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/wan2.2_i2v_high_ulitmate_pussy_asshole.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/wan2.2_i2v_low_ulitmate_pussy_asshole.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/wan22-mouthfull-140epoc-high-k3nk.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/wan22-mouthfull-152epoc-low-k3nk.safetensors"
  "https://huggingface.co/Zachimo/f4c3spl4sh/resolve/main/wan22-f4c3spl4sh-100epoc-high-k3nk.safetensors"
  "https://huggingface.co/Zachimo/f4c3spl4sh/resolve/main/wan22-f4c3spl4sh-154epoc-low-k3nk.safetensors"
  "https://huggingface.co/NikolaSigmoid/wan2.2-i2v-loras-fingering/resolve/main/highnoise.safetensors"
  "https://huggingface.co/NikolaSigmoid/wan2.2-i2v-loras-fingering/resolve/main/lownoise.safetensors"
  "https://huggingface.co/FataleCherry/Hi_LickingLips/resolve/main/LipL-high-60%20(1).safetensors"
  "https://huggingface.co/FataleCherry/Low_LickingLips/resolve/main/LipL-low-60%20(1).safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/Pornmaster_wan%202.2_14b_I2V_bukkake_v1.4_high_noise.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/Pornmaster_wan%202.2_14b_I2V_bukkake_v1.4_low_noise.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/W22_Multiscene_Photoshoot_Softcore_i2v_HN.safetensors"
  "https://huggingface.co/lkzd7/WAN2.2_LoraSet_NSFW/resolve/main/W22_Multiscene_Photoshoot_Softcore_i2v_LN.safetensors"
  "https://huggingface.co/Kijai/WanVideo_comfy/resolve/main/LoRAs/Stable-Video-Infinity/v2.0/SVI_v2_PRO_Wan2.2-I2V-A14B_LOW_lora_rank_128_fp16.safetensors"
  "https://huggingface.co/Kijai/WanVideo_comfy/resolve/main/LoRAs/Stable-Video-Infinity/v2.0/SVI_v2_PRO_Wan2.2-I2V-A14B_HIGH_lora_rank_128_fp16.safetensors"
  "https://huggingface.co/lightx2v/Wan2.2-Distill-Loras/resolve/main/wan2.2_t2v_A14b_low_noise_lora_rank64_lightx2v_4step_1217.safetensors"
  "https://huggingface.co/lightx2v/Wan2.2-Distill-Loras/resolve/main/wan2.2_t2v_A14b_high_noise_lora_rank64_lightx2v_4step_1217.safetensors"
  "https://huggingface.co/lightx2v/Wan2.2-Distill-Loras/resolve/main/wan2.2_i2v_A14b_high_noise_lora_rank64_lightx2v_4step_1022.safetensors"
  "https://huggingface.co/lightx2v/Wan2.2-Distill-Loras/resolve/main/wan2.2_i2v_A14b_low_noise_lora_rank64_lightx2v_4step_1022.safetensors"
  "https://huggingface.co/Kijai/WanVideo_comfy/resolve/main/Lightx2v/lightx2v_I2V_14B_480p_cfg_step_distill_rank128_bf16.safetensors"
)

VAE_MODELS=(
  "https://huggingface.co/Comfy-Org/Wan_2.1_ComfyUI_repackaged/resolve/main/split_files/vae/wan_2.1_vae.safetensors"
)

ESRGAN_MODELS=(
)

DIFFUSION_MODELS=(
  "https://huggingface.co/LiconStudio/VBVR-wan2.2-comfy-bf16/resolve/main/VBVR-wan2.2-comfy-high-bf16.safetensors"
  "https://huggingface.co/LiconStudio/VBVR-wan2.2-comfy-bf16/resolve/main/VBVR-wan2.2-comfy-low-bf16.safetensors"
  "https://huggingface.co/xroli/DasiwaWAN22I2V14BLightspeed_synthseductionHighV9/resolve/main/DasiwaWAN22I2V14BLightspeed_synthseductionHighV9.safetensors"
  "https://huggingface.co/xroli/DasiwaWAN22I2V14BLightspeed_synthseductionHighV9/resolve/main/DasiwaWAN22I2V14BLightspeed_synthseductionLowV9.safetensors"
)

CONTROLNET_MODELS=(
)

TEXT_ENCODERS_MODELS=(
  "https://huggingface.co/Comfy-Org/Wan_2.1_ComfyUI_repackaged/resolve/main/split_files/text_encoders/umt5_xxl_fp8_e4m3fn_scaled.safetensors"
  "https://huggingface.co/NSFW-API/NSFW-Wan-UMT5-XXL/resolve/main/nsfw_wan_umt5-xxl_fp8_scaled.safetensors"
)

### DO NOT EDIT BELOW HERE UNLESS YOU KNOW WHAT YOU ARE DOING ###

function provisioning_start() {
    provisioning_print_header
    provisioning_get_apt_packages
    provisioning_get_nodes
    provisioning_get_pip_packages
    provisioning_get_files \
        "${COMFYUI_DIR}/models/checkpoints" \
        "${CHECKPOINT_MODELS[@]}"
    provisioning_get_files \
        "${COMFYUI_DIR}/models/unet" \
        "${UNET_MODELS[@]}"
    provisioning_get_files \
        "${COMFYUI_DIR}/models/lora" \
        "${LORA_MODELS[@]}"
    provisioning_get_files \
        "${COMFYUI_DIR}/models/controlnet" \
        "${CONTROLNET_MODELS[@]}"
    provisioning_get_files \
        "${COMFYUI_DIR}/models/vae" \
        "${VAE_MODELS[@]}"
    provisioning_get_files \
        "${COMFYUI_DIR}/models/esrgan" \
        "${ESRGAN_MODELS[@]}"
    provisioning_get_files \
        "${COMFYUI_DIR}/models/diffusion_models" \
        "${DIFFUSION_MODELS[@]}"
    provisioning_get_files \
        "${COMFYUI_DIR}/models/text_encoders" \
        "${TEXT_ENCODERS_MODELS[@]}"
    provisioning_print_end
}

function provisioning_get_apt_packages() {
    if [[ -n $APT_PACKAGES ]]; then
            sudo $APT_INSTALL ${APT_PACKAGES[@]}
    fi
}

function provisioning_get_pip_packages() {
    if [[ -n $PIP_PACKAGES ]]; then
            pip install --no-cache-dir ${PIP_PACKAGES[@]}
    fi
}

function provisioning_get_nodes() {
    for repo in "${NODES[@]}"; do
        dir="${repo##*/}"
        path="${COMFYUI_DIR}custom_nodes/${dir}"
        requirements="${path}/requirements.txt"
        if [[ -d $path ]]; then
            if [[ ${AUTO_UPDATE,,} != "false" ]]; then
                printf "Updating node: %s...\n" "${repo}"
                ( cd "$path" && git pull )
                if [[ -e $requirements ]]; then
                   pip install --no-cache-dir -r "$requirements"
                fi
            fi
        else
            printf "Downloading node: %s...\n" "${repo}"
            git clone "${repo}" "${path}" --recursive
            if [[ -e $requirements ]]; then
                pip install --no-cache-dir -r "${requirements}"
            fi
        fi
    done
}

function provisioning_get_files() {
    if [[ -z $2 ]]; then return 1; fi
    
    dir="$1"
    mkdir -p "$dir"
    shift
    arr=("$@")
    printf "Downloading %s model(s) to %s...\n" "${#arr[@]}" "$dir"
    for url in "${arr[@]}"; do
        printf "Downloading: %s\n" "${url}"
        provisioning_download "${url}" "${dir}"
        printf "\n"
    done
}

function provisioning_print_header() {
    printf "\n##############################################\n#                                            #\n#          Provisioning container            #\n#                                            #\n#         This will take some time           #\n#                                            #\n# Your container will be ready on completion #\n#                                            #\n##############################################\n\n"
}

function provisioning_print_end() {
    printf "\nProvisioning complete:  Application will start now\n\n"
}

function provisioning_has_valid_hf_token() {
    [[ -n "$HF_TOKEN" ]] || return 1
    url="https://huggingface.co/api/whoami-v2"

    response=$(curl -o /dev/null -s -w "%{http_code}" -X GET "$url" \
        -H "Authorization: Bearer $HF_TOKEN" \
        -H "Content-Type: application/json")

    # Check if the token is valid
    if [ "$response" -eq 200 ]; then
        return 0
    else
        return 1
    fi
}

function provisioning_has_valid_civitai_token() {
    [[ -n "$CIVITAI_TOKEN" ]] || return 1
    url="https://civitai.com/api/v1/models?hidden=1&limit=1"

    response=$(curl -o /dev/null -s -w "%{http_code}" -X GET "$url" \
        -H "Authorization: Bearer $CIVITAI_TOKEN" \
        -H "Content-Type: application/json")

    # Check if the token is valid
    if [ "$response" -eq 200 ]; then
        return 0
    else
        return 1
    fi
}

# Download from $1 URL to $2 file path
function provisioning_download() {
    if [[ -n $HF_TOKEN && $1 =~ ^https://([a-zA-Z0-9_-]+\.)?huggingface\.co(/|$|\?) ]]; then
        auth_token="$HF_TOKEN"
    elif 
        [[ -n $CIVITAI_TOKEN && $1 =~ ^https://([a-zA-Z0-9_-]+\.)?civitai\.com(/|$|\?) ]]; then
        auth_token="$CIVITAI_TOKEN"
    fi
    if [[ -n $auth_token ]];then
        wget --header="Authorization: Bearer $auth_token" -qnc --content-disposition --show-progress -e dotbytes="${3:-4M}" -P "$2" "$1"
    else
        wget -qnc --content-disposition --show-progress -e dotbytes="${3:-4M}" -P "$2" "$1"
    fi
}

# Allow user to disable provisioning if they started with a script they didn't want
if [[ ! -f /.noprovisioning ]]; then
    provisioning_start
fi
