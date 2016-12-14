# AudioUnit
AudioUnit PLAY AND RECORD
Codes copy from GOOGLE CODES web site.

support voiceprocessingIO
  // Describe audio component
    AudioComponentDescription desc;
    desc.componentType = kAudioUnitType_Output;
    if([AssertSDK isValidechoCancellation4Connecting:@""]){
        desc.componentSubType = kAudioUnitSubType_VoiceProcessingIO;
        NSLog(@"VoicePIO--------->LTVideoSDK INFOs");
    }else{
        desc.componentSubType = kAudioUnitSubType_RemoteIO;
        NSLog(@"VoiceRIO--------->LTVideoSDK INFOs");
    }
    desc.componentFlags = 0;
    desc.componentFlagsMask = 0;
    desc.componentManufacturer = kAudioUnitManufacturer_Apple;
