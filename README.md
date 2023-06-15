# gha-serverless-with-python-requirements
Javascript action that runs a Serverless deploy using the serverless-python-requirements plugin.

node version 16
serverless@2.72.3

using:

      - name: Serverless Deploy
        uses: yavinenana/gha-serverless-with-python-requirements@v2.0.3
        with:
          args: '--stage qa --region $REGION'
        env:
          AWS_ACCESS_KEY_ID: ${{ secrets.AWS_ACCESS_KEY_ID_QA }}
          AWS_SECRET_ACCESS_KEY: ${{ secrets.AWS_SECRET_ACCESS_KEY_QA }}
          REGION: ${{ secrets.AWS_REGION_QA }}
