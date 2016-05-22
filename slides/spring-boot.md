##  Spring Boot
#### finally!
```
@Configuration
@Profile("hazelcast")
public class HazelcastConfiguration implements CachingConfigurer {

	@Value("${hz_url}")
	private String hazelCastManagementUrl;

	@Value("${hz_members}")
	private String hazelcastMembers;

	@Bean
	public Config hazelcastConfig(){
		Config config = new Config();
		NetworkConfig networkConfig = config.getNetworkConfig();
		networkConfig.setPort(5901);
```

note:
1. death to xml
1. configuration as code
1. true write once
1. boilerplate done
1. embedded container
