
pipeline
{
	agent any
	stages
	{
		stage("Create Directory")
		{
			steps
			{
				sh 'mkdir MyFolder'
				echo "Folder Has Been Created"
			}
		}
		
		stage("Create File")
		{
			steps
			{
				script
				{
					dir("MyFolder")
					{
						sh 'touch MyFile.txt'
						echo "File Has Been Created"
					}
				}
			}
		}
		
		stage("Write File")
		{
			steps
			{
				script
				{
					dir("MyFolder")
					{
						sh 'echo "Hello From Git" > MyFile.txt'
						echo "File Has Been Writted"
					}
				}
			}
		}

	}
}
