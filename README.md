% Matlabでの簡単な数字当てゲーム

% 1から100のランダムな整数を生成
target_number = randi([1, 100]);

fprintf('1から100の範囲の整数を当ててください。\n');

while true
    % ユーザーに数字を入力させる
    guess = input('予想した数字を入力してください: ');

    % 入力された数字と目標の数字を比較
    if guess == target_number
        fprintf('おめでとうございます！正解です。\n');
        break;
    elseif guess < target_number
        fprintf('もっと大きな数字です。\n');
    else
        fprintf('もっと小さな数字です。\n');
    end
end
