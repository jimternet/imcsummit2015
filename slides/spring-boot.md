##  Spring Boot
#### finally! 
```
@Configuration
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
		networkConfig.setPortAutoIncrement(false);
		JoinConfig join = networkConfig.getJoin();
```
