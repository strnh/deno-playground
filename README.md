# deno + snowpack

* requirement: npm/yarn 

```sh
% npm install deno snowpack 
% yarn add snowpack 
% yarn run snowpack init
yarn run v1.22.19
warning package.json: No license field
$ /home/strnh/node_modules/.bin/snowpack init
[13:19:08] [snowpack] Hint: run "snowpack init" to create a project config file. Using defaults...
[13:19:08] [snowpack] Creating new project configuration file... (snowpack.config.js)
[13:19:08] [snowpack] File created! Open snowpack.config.js to customize your project.
Done in 0.32s.
% % yarn run snowpack dev
yarn run v1.22.19
warning package.json: No license field
$ /home/strnh/node_modules/.bin/snowpack dev
[13:22:00] [snowpack] Welcome to Snowpack! Because this is your first time running
this project, Snowpack needs to prepare your dependencies. This is a one-time step
and the results will be cached for the lifetime of your project. Please wait...

<--- Last few GCs --->
<--- Last few GCs --->

[168487:0x35625000]    52920 ms: Mark-Compact 3976.3 (4146.4) -> 3976.3 (4141.4) MB, pooled: 50 MB, 242.52 / 0.00 ms  (average mu = 0.117, current mu = 0.038) allocation failure; scavenge might not succeed
[168487:0x35625000]    53169 ms: Mark-Compact 3983.8 (4148.9) -> 3983.7 (4144.1) MB, pooled: 54 MB, 239.86 / 0.00 ms  (average mu = 0.078, current mu = 0.038) allocation failure; scavenge might not succeed


<--- JS stacktrace --->

FATAL ERROR: Reached heap limit Allocation failed - JavaScript heap out of memory
----- Native stack trace -----

 1: 0xe3811e node::OOMErrorHandler(char const*, v8::OOMDetails const&) [/usr/local/bin/node]
 2: 0x125fb70 v8::Utils::ReportOOMFailure(v8::internal::Isolate*, char const*, v8::OOMDetails const&) [/usr/local/bin/node]
 3: 0x125fe47 v8::internal::V8::FatalProcessOutOfMemory(v8::internal::Isolate*, char const*, v8::OOMDetails const&) [/usr/local/bin/node]
 4: 0x148d885  [/usr/local/bin/node]
 5: 0x14a70f9 v8::internal::Heap::CollectGarbage(v8::internal::AllocationSpace, v8::internal::GarbageCollectionReason, v8::GCCallbackFlags) [/usr/local/bin/node]
 6: 0x147b7c8 v8::internal::HeapAllocator::AllocateRawWithLightRetrySlowPath(int, v8::internal::AllocationType, v8::internal::AllocationOrigin, v8::internal::AllocationAlignment) [/usr/local/bin/node]
 7: 0x147c6f5 v8::internal::HeapAllocator::AllocateRawWithRetryOrFailSlowPath(int, v8::internal::AllocationType, v8::internal::AllocationOrigin, v8::internal::AllocationAlignment) [/usr/local/bin/node]
 8: 0x1454aee v8::internal::Factory::AllocateRaw(int, v8::internal::AllocationType, v8::internal::AllocationAlignment) [/usr/local/bin/node]
 9: 0x1443be4 v8::internal::FactoryBase<v8::internal::Factory>::AllocateRawWithImmortalMap(int, v8::internal::AllocationType, v8::internal::Tagged<v8::internal::Map>, v8::internal::AllocationAlignment) [/usr/local/bin/node]
10: 0x1445aef v8::internal::FactoryBase<v8::internal::Factory>::NewRawTwoByteString(int, v8::internal::AllocationType) [/usr/local/bin/node]
11: 0x14604ca v8::internal::Factory::NewStringFromUtf8(v8::base::Vector<char const>, v8::internal::AllocationType) [/usr/local/bin/node]
12: 0x127c08d v8::String::NewFromUtf8(v8::Isolate*, char const*, v8::NewStringType, int) [/usr/local/bin/node]
13: 0x10ef759  [/usr/local/bin/node]
14: 0xf64dbd  [/usr/local/bin/node]
15: 0x71133adcf745 
Aborted (core dumped)
error Command failed with exit code 134.
info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.

```
