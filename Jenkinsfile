//
// Jenkinsfile
//
// Jenkins pipeline file for Example Docker image builds. This defines the
// Jenkins job that builds your Docker image.
//
// @author Nick Hentschel <nhentschel@wayfair.com>
// @copyright 2018 Wayfair, LLC. -- All rights reserved.

@Library('jenkins-pipeline-library') _

dockerBuildPipeline {
  // Optional parameters below affect builds. All settings have defaults, and
  // it's highly likely the defaults will work for you. Uncomment anything you
  // need to change.

  // buildsToKeep = 25         // Number of builds to store in job history, must be an integer.
  // imagesToSkip = []         // Images that should be skipped for CI builds.
  // rebuildAll   = false      // Whether to rebuild all images every time a commit is pushed.
  // runGossTests = true       // Whether Goss tests should be run.
  // skipPublish  = false      // Whether the publishing of images should be skipped. Useful for testing.
  // slaveLabel   = 'ci'       // Slave label to build on.
  // tagStrategy  = 'semantic' // Set the container tagging policy. Can be either 'semantic' or 'sha',
                               // is set to 'semantic' by default

  // Extreme caution should be used with the following parameters. They affect
  // Jenkins job build parameters and should be used in exceptional cases.

  // latestTag = false         // Should we also update the 'latest' tag on push?

  // tagOverride = ''          // Ignore tagStrategy and set this tag exactly.
  // triggerOn = 'scm'         // Jenkins job trigger, supported values are: 'scm', 'cron'
  // triggerCron = 'H * * * *' // In case of 'cron' trigger, specifies the schedule.

  // preBuildSvc = []          // Docker-compose services to be executed before the build.
  // preBuildTimeout = 5       // Timeout for all pre-build steps in minutes.
  // postBuildSvc = []         // Docker-compose services to be executed after the build.
  // postBuildTimeout = 5      // Timeout for all post-build steps in minutes.
}
