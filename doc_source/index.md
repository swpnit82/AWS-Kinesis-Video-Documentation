# Amazon Kinesis Video Streams Developer Guide

-----
*****Copyright &copy; 2020 Amazon Web Services, Inc. and/or its affiliates. All rights reserved.*****

-----
Amazon's trademarks and trade dress may not be used in 
     connection with any product or service that is not Amazon's, 
     in any manner that is likely to cause confusion among customers, 
     or in any manner that disparages or discredits Amazon. All other 
     trademarks not owned by Amazon are the property of their respective
     owners, who may or may not be affiliated with, connected to, or 
     sponsored by Amazon.

-----
## Contents
+ [What Is Amazon Kinesis Video Streams?](what-is-kinesis-video.md)
+ [Kinesis Video Streams System Requirements](system-requirements.md)
+ [Amazon Kinesis Video Streams: How It Works](how-it-works.md)
   + [Kinesis Video Streams API and Producer Libraries Support](how-it-works-kinesis-video-api-producer-sdk.md)
   + [Kinesis Video Streams Playback](how-playback.md)
      + [Video Playback with HLS](hls-playback.md)
      + [Video Playback with MPEG-DASH](dash-playback.md)
   + [Using Streaming Metadata with Kinesis Video Streams](how-meta.md)
   + [Kinesis Video Streams Data Model](how-data.md)
+ [Getting Started with Kinesis Video Streams](getting-started.md)
   + [Step 1: Set Up an AWS Account and Create an Administrator](gs-account.md)
   + [Step 2: Create a Kinesis Video Stream](gs-createstream.md)
   + [Step 3: Send Data to a Kinesis Video Stream](gs-send-data.md)
   + [What's Next?](gs-console-whatnext.md)
+ [Security in Amazon Kinesis Video Streams](security.md)
   + [Data Protection in Kinesis Video Streams](how-kms.md)
   + [Controlling Access to Kinesis Video Streams Resources Using IAM](how-iam.md)
   + [Controlling Access to Kinesis Video Streams Resources Using AWS IoT](how-iot.md)
   + [Monitoring Amazon Kinesis Video Streams](security-monitoring.md)
   + [Compliance Validation for Amazon Kinesis Video Streams](akda-java-compliance.md)
   + [Resilience in Amazon Kinesis Video Streams](disaster-recovery-resiliency.md)
   + [Infrastructure Security in Kinesis Video Streams](infrastructure-security.md)
   + [Security Best Practices for Kinesis Video Streams](security-best-practices.md)
+ [Kinesis Video Streams Producer Libraries](producer-sdk.md)
   + [Using the Java Producer Library](producer-sdk-javaapi.md)
      + [Step 1: Download and Configure the Java Producer Library Code](producersdk-javaapi-downloadcode.md)
      + [Step 2: Write and Examine the Code](producersdk-javaapi-writecode.md)
      + [Step 3: Run and Verify the Code](producersdk-javaapi-reviewcode.md)
   + [Using the Android Producer Library](producer-sdk-android.md)
      + [Step 1: Download and Configure the Android Producer Library Code](producersdk-android-downloadcode.md)
      + [Step 2: Examine the Code](producersdk-android-writecode.md)
      + [Step 3: Run and Verify the Code](producersdk-android-reviewcode.md)
   + [Using the C++ Producer Library](producer-sdk-cpp.md)
      + [Step 1: Download and Configure the C++ Producer Library Code](producersdk-cpp-download.md)
      + [Step 2: Write and Examine the Code](producersdk-cpp-write.md)
      + [Step 3: Run and Verify the Code](producersdk-cpp-test.md)
      + [Using the C++ Producer SDK as a GStreamer Plugin](producer-sdk-cpp-gstreamer.md)
      + [Using the C++ Producer SDK as a GStreamer Plugin in a Docker Container](producer-sdk-cpp-gstreamer-docker.md)
      + [Using the C++ Producer SDK on Windows](producer-sdk-win.md)
      + [Using the C++ Producer SDK on Raspberry Pi](producersdk-cpp-rpi.md)
      + [Using Logging with the C++ Producer SDK](producer-sdk-cpp-logging.md)
   + [Using the C Producer Library](producer-sdk-c-api.md)
      + [Step 1: Download the C Producer Library Code](producersdk-c-download.md)
      + [Step 2: Write and Examine the Code](producersdk-c-write.md)
      + [Step 3: Run and Verify the Code](producersdk-c-test.md)
   + [Producer SDK Reference](producer-reference.md)
      + [Producer SDK Limits](producer-sdk-limits.md)
      + [Error Code Reference](producer-sdk-errors.md)
      + [Network Abstraction Layer (NAL) Adaptation Flag Reference](producer-reference-nal.md)
      + [Producer SDK Structures](producer-reference-structures-producer.md)
      + [Kinesis Video Stream Structures](producer-reference-structures-stream.md)
      + [Producer SDK Callbacks](producer-reference-callbacks.md)
+ [Kinesis Video Stream Parser Library](parser-library.md)
   + [Step 1: Download and Configure the Code](parser-library-download.md)
   + [Step 2: Write and Examine the Code](parser-library-write.md)
   + [Step 3: Run and Verify the Code](parser-library-run.md)
+ [Amazon Kinesis Video Streams Examples](examples.md)
   + [Example: Kinesis Video Streams Producer SDK GStreamer Plugin](examples-gstreamer-plugin.md)
      + [GStreamer Element Parameter Reference](examples-gstreamer-plugin-parameters.md)
   + [Example: Sending Data to Kinesis Video Streams Using the PutMedia API](examples-putmedia.md)
   + [Example: Streaming from an RTSP Source](examples-rtsp.md)
   + [Example: Parsing and Rendering Kinesis Video Streams Fragments](examples-renderer.md)
   + [Example: Identifying Objects in Video Streams Using Amazon SageMaker](examples-sagemaker.md)
+ [Monitoring Kinesis Video Streams](monitoring.md)
   + [Monitoring Kinesis Video Streams Metrics with CloudWatch](monitoring-cloudwatch.md)
   + [Logging Kinesis Video Streams API Calls with AWS CloudTrail](monitoring-cloudtrail.md)
+ [Kinesis Video Streams Limits](limits.md)
+ [Troubleshooting Kinesis Video Streams](troubleshooting.md)
+ [Document History for Amazon Kinesis Video Streams](doc-history.md)
+ [API Reference](API_Reference.md)
   + [Actions](API_Operations.md)
      + [Amazon Kinesis Video Streams](API_Operations_Amazon_Kinesis_Video_Streams.md)
         + [CreateSignalingChannel](API_CreateSignalingChannel.md)
         + [CreateStream](API_CreateStream.md)
         + [DeleteSignalingChannel](API_DeleteSignalingChannel.md)
         + [DeleteStream](API_DeleteStream.md)
         + [DescribeSignalingChannel](API_DescribeSignalingChannel.md)
         + [DescribeStream](API_DescribeStream.md)
         + [GetDataEndpoint](API_GetDataEndpoint.md)
         + [GetSignalingChannelEndpoint](API_GetSignalingChannelEndpoint.md)
         + [ListSignalingChannels](API_ListSignalingChannels.md)
         + [ListStreams](API_ListStreams.md)
         + [ListTagsForResource](API_ListTagsForResource.md)
         + [ListTagsForStream](API_ListTagsForStream.md)
         + [TagResource](API_TagResource.md)
         + [TagStream](API_TagStream.md)
         + [UntagResource](API_UntagResource.md)
         + [UntagStream](API_UntagStream.md)
         + [UpdateDataRetention](API_UpdateDataRetention.md)
         + [UpdateSignalingChannel](API_UpdateSignalingChannel.md)
         + [UpdateStream](API_UpdateStream.md)
      + [Amazon Kinesis Video Streams Media](API_Operations_Amazon_Kinesis_Video_Streams_Media.md)
         + [GetMedia](API_dataplane_GetMedia.md)
         + [PutMedia](API_dataplane_PutMedia.md)
      + [Amazon Kinesis Video Streams Archived Media](API_Operations_Amazon_Kinesis_Video_Streams_Archived_Media.md)
         + [GetClip](API_reader_GetClip.md)
         + [GetDASHStreamingSessionURL](API_reader_GetDASHStreamingSessionURL.md)
         + [GetHLSStreamingSessionURL](API_reader_GetHLSStreamingSessionURL.md)
         + [GetMediaForFragmentList](API_reader_GetMediaForFragmentList.md)
         + [ListFragments](API_reader_ListFragments.md)
      + [Amazon Kinesis Video Signaling Channels](API_Operations_Amazon_Kinesis_Video_Signaling_Channels.md)
         + [GetIceServerConfig](API_AWSAcuitySignalingService_GetIceServerConfig.md)
         + [SendAlexaOfferToMaster](API_AWSAcuitySignalingService_SendAlexaOfferToMaster.md)
   + [Data Types](API_Types.md)
      + [Amazon Kinesis Video Streams](API_Types_Amazon_Kinesis_Video_Streams.md)
         + [ChannelInfo](API_ChannelInfo.md)
         + [ChannelNameCondition](API_ChannelNameCondition.md)
         + [ResourceEndpointListItem](API_ResourceEndpointListItem.md)
         + [SingleMasterChannelEndpointConfiguration](API_SingleMasterChannelEndpointConfiguration.md)
         + [SingleMasterConfiguration](API_SingleMasterConfiguration.md)
         + [StreamInfo](API_StreamInfo.md)
         + [StreamNameCondition](API_StreamNameCondition.md)
         + [Tag](API_Tag.md)
      + [Amazon Kinesis Video Streams Media](API_Types_Amazon_Kinesis_Video_Streams_Media.md)
         + [StartSelector](API_dataplane_StartSelector.md)
      + [Amazon Kinesis Video Streams Archived Media](API_Types_Amazon_Kinesis_Video_Streams_Archived_Media.md)
         + [ClipFragmentSelector](API_reader_ClipFragmentSelector.md)
         + [ClipTimestampRange](API_reader_ClipTimestampRange.md)
         + [DASHFragmentSelector](API_reader_DASHFragmentSelector.md)
         + [DASHTimestampRange](API_reader_DASHTimestampRange.md)
         + [Fragment](API_reader_Fragment.md)
         + [FragmentSelector](API_reader_FragmentSelector.md)
         + [HLSFragmentSelector](API_reader_HLSFragmentSelector.md)
         + [HLSTimestampRange](API_reader_HLSTimestampRange.md)
         + [TimestampRange](API_reader_TimestampRange.md)
      + [Amazon Kinesis Video Signaling Channels](API_Types_Amazon_Kinesis_Video_Signaling_Channels.md)
         + [IceServer](API_AWSAcuitySignalingService_IceServer.md)
   + [Common Errors](CommonErrors.md)
   + [Common Parameters](CommonParameters.md)