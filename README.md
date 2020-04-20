# Spectral With JSON Output

In this example you'll see how to use a JSON output in addition to your regular stylish reporter.

This is great for cases where you want to ship logs to your SIEM system or your log management service.

You need to use Spectral v1.9x series (vNext: `curl -L spectralops.io/next | sh`).

Look in [.spectral/spectral.yaml](.spectral/spectral.yaml):

    reporter:
        outputs:
            stylish: {}        # nice looking CLI reports
            log:              # use a logger
                json: true      # enable JSON logging
                file: out.json  # put output in a file

